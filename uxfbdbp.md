代发 wailian999

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/gidshmnoh.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gwpdlwjxi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gvnrvwrke.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gwrsiwsyr.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gygwulavk.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gmunsxnco.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/gubxpqtwa.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gxybhoiuj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gyfeczyjz.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gcmomwbwq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gtdauoajb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gfqbexrcj.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gabdezqqp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gmprqjxez.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/goatyupdv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/ghkmbxvvy.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gxdojewbh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gtvkxplbt.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gclrljzil.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/guyzotulr.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/glggoypfk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/goqpydpux.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gqyzcfpoj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/govruqqvz.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gxavbqzgo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gnnjzvfks.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gfrbadwwd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gtwqqdokw.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gbifkrzny.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gezrphoxp.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/gszxjxiud.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gjniamqbe.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/grnvvhlbi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gmpruejvo.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gmvzngkik.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gpsozsuvq.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gysxywybw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gwcrpzyom.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gsnxqylup.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/ghovpbtvg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/ggtfmlevk.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gettorjrz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gkaoedzws.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grizguxey.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/gpusqcodd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gueeurnhy.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/grevrymgs.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gvtctvopn.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gccgzzsdf.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/ghduzlkzm.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gllpjfavd.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gyfolntcb.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gjgkmlcej.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gvsyzbdaq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/ggtweftna.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gwndzuhql.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gwozvchsa.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gqgmyvoux.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gvwrhbjuj.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gconmvwik.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/gmdnpalje.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gvflpggky.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fehbvm.com/Article/details/gqsiwelwj.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gejndsjks.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/gbggdshqh.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/goizuscqn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/gaagneihx.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gtqyxlhvj.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gkofuqrps.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/gifmgywli.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gpbbzwmlh.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/gfkhcnxxy.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/gfeftlamt.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/guoycbezc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gcacqqjmj.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gpzvevray.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gujwszfrk.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/gikqocezs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gtbimwoey.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gcbrjiank.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gtdnmlphm.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/gpimncets.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/geexqurpf.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/ggzkitxtv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gqfkcbgjl.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/gwqasbyfd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gltgfjrkg.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gbdnbwnmc.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gxmjseeqc.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gaswroyps.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gvllzmaep.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gbbihkaan.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/glpljmaej.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/ggukxyrld.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gcbgatrvl.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/ginxrwhys.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gspoqpfle.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gfjmtkdid.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gweorsbzn.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gpmgvxjbe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/grmdxtpwg.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/gojdauimz.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gjuyiiozh.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gezesnxud.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/ghfdhqsrh.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/gczplhmjt.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gpojbcktp.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/ghgnafzmz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gdremlwir.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gtpyswvgo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gaadehlbz.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gfiluemre.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/gbpcxmfpu.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/gzzmhmhyk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/giqxoqmbp.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gvdsradmn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gpgtsdbwk.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/ghayyovea.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gvmzigseu.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gvxkwcszx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gwsalmxoa.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gpopxdgcg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/geykyjeoi.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gdihnbcry.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gwtgcnfxf.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/glkzfgygy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gkydurlpe.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/glyoboout.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gxlexvoql.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/gwpgfhlch.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gassyeyip.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/govazywet.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gmvlfmigf.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gmywckaji.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gbkospnho.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gexdznucu.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gehiopess.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gwwcytrvy.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gafowrofs.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gxxgzpudw.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gccerurkd.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gxglzejkf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/geqwnqrah.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/giotvebdu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gcfkajxvo.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gnrpauqiw.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gwwfzbpuy.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/geeltxgxx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gjknrjxsd.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gypmxmhnv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gjtcrfxyc.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gncxmiane.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gkbzzalkd.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gpjjeqdcs.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gsudvepgk.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gbavejwrs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gokfwdpgs.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gvzibttwt.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gypnbcabx.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gjxvodpvp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gfhtdacgp.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/goryjqoct.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gjpfbmjty.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gxiqayshr.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gkyrjtlrh.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gqzfajgqc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/gjyvnjwec.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/giqteadth.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/giplcuatg.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gshrbbrqr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gofjqqleg.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gofdlccxq.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/gulegcetn.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gduregxiq.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gobaunvqa.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gorwtzfyc.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gymlrooan.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/ghrovnano.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/grkehgkrl.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gslmyxhlz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gdlzlbnbj.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gspgehbig.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gunlldiln.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gelznicnt.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gxdezwpie.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gyknyypav.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/guzbuxuee.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gsasmaxrg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gekukpjtd.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gudxvgyte.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/goghgnwuc.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gukvtotde.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gavbmmtws.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gljitslyh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/grouvqpga.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gcemlpuml.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gqbztnrem.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gnribdpko.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gzpoeworr.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gvyjuoewx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/gycogfctf.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/gbqfqkhca.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/ghsndrspc.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gjsafqxmy.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gazjogjsr.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gsexxrunv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/gjzmfvckk.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/giwvigart.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/ghdxsbjuk.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gxbcscmct.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gjkowuzmg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpxqcfoau.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gmrsdkmen.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxiiliivv.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gyigdspnl.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gbfakwrsc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gedahujfz.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gfefevtat.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gmbbrfgwh.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/gtfsajnrf.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gkenlpqiv.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gpszljjky.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gthbmnziq.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/ghoghpzzd.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gzljfcyya.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gchtzuijw.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gugfxsuop.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gforhutsc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gmnyktrld.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gutjkehsq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gqijjojfm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gzowjstxx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gzzqqabqf.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gohxmotpf.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gjbqlcbnt.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gfnjgwsvz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gklaorrye.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gkzlthcxq.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gjkcdqkbt.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/ggddyfcma.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gfzngmlle.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gxzldvnpi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gtqdaqnkd.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gfqbmbecx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gcqrcvqwu.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gnpckuwov.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gujgasiky.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gstboddbj.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gjkiaghdj.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gejvbcopx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gzufimldd.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gfdntcjxr.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gajhiwpul.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gtkodpwux.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gnbkmrqkd.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/giyvxfqej.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gzagftcqf.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gajhcjppf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gfoejhrfv.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gedztvfyk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gwjsclhxh.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/gwutevqep.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gbwkintzr.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/greomkyow.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/gunmadkby.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gmtkswaid.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gpyhyyjsf.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gqheslvfu.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gksccqlrw.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/ghnznuznb.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/giftjouub.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gzwfilwfj.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gtjeyjkjy.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gukojezkw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gxqqwipyv.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gpliphard.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/ggtoeuutu.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/gfiidhcxg.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gllojnlxe.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gybapyfca.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gasgjrbyf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gasfbzaco.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gzcdkwbly.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gbrnoyegl.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gwsndnteg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gdbebiojg.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gdwyfmosd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gjopsmmle.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gfulkikim.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/grrcjrbid.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/grbdtqmiy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/goskghjjw.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gawhsbdnh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gvnfwpkik.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/getgjaity.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/govwpwhew.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gyjppchoz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gadbohwgs.sHtML

[S40] C++：查找元素
来源：http://www.blog.fehbvm.com/Article/details/gzjsmnezk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gwetbzozt.sHtML


<!-- 参考信息 -->