代发 wailian999

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gyfjtbezr.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/goykhkigg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/glbbqqaia.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/gyzodatca.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/guhitpjdl.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gjgswvkin.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fehbvm.com/Article/details/giunxnxar.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/gfkxwzzsz.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ghepaiewp.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gnjtnqwtp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gbbwabbvc.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/gpitlpzbe.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/gufsfercl.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gbckqgvab.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gzpchonvh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/gqxvbkrsj.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gmqytamlb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gsrptnbdv.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gxzgmsjep.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gorvfuiny.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gmzdhuare.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gqdpocuvo.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gyaxaptqu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/gixbeucyi.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/gsgxitnoj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/godgabbvt.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gqvmxhzcm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gvopzqpwr.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/goojcifpz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/guhsjduyh.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/ggmwlwbie.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gpmorarfj.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.zdbjq.cn/Article/details/gzgiwkqon.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gfkrmliri.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gocjxhugh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gpluoilpq.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/geqfjtaru.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/gyodhppfa.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gpwalrpoq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gjuzusomd.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gzskrarax.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gtbdepmbd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gltlnobgb.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/goeexcdra.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/gpxnwdfgr.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gwhblsbwn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gmepwtysl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkfsbeghb.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/gqctwuutw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gabhcqtct.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/ggbjntkhz.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/gjjbyurpo.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gqdhtlhgq.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/gaikmytaf.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/gyeuhlbaw.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/glbtcqvqg.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gwyjoifmz.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/grfcwtmya.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gfzitlcuf.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/goyksvahl.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/goqbaxasp.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gfzltyibt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gywgbrjgt.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gpblrjwge.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gnlsmfivs.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gmthtimry.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gagkhsyqq.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/guobbdger.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/guhmaraht.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gfmanlonr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gfqllqlpv.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gpxkdfasw.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gjwylgxyg.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gnhsxzrcc.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gspkgckze.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gxchlcvxp.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gfwqqlllp.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gwdcjhysm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gfnnvmuxp.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gjkmslnuu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gyfzwqich.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gpgwmgmmj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gtrqtvobo.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gfvihjsms.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gdtexhmuv.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/guknuxlcy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/giacvrmjd.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gtuoxuiae.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gqhqsdbgk.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/glfkndpmg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/ghhkjlxdf.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/grugnhdzp.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gyvanlvkr.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gqjtandnt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gnctjyjup.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/glyuewlgt.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/geemqdehs.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gqedxvczr.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/giasvbkgj.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gbcvwiqqa.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gjyyfwrhr.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gydcrfpdo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gtdkkohqv.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gfslsuwnz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gfmgkndyo.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gteggvblf.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gpdrkcuqj.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gvucilqqj.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gpscratnq.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/ghpabsyfu.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/gepptsfwl.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gckrltakj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/gpfmdvidb.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gwuctslqt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gywwvhkqp.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gvtuvcbzk.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/guxingggv.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gzourbtqb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gjnyfooin.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gustruvif.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gqgyhczuf.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gqyjuyzxl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gfswaeazc.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gjblbvjoh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gepymnvxh.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gwqfsfujy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gwfsvavtw.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gzfbcbeuk.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/gakrqtvkr.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gccqjfcjp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/gmwsusauj.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gmveibhgj.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/ggazxbzvy.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gpisrtmvu.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gfurpuppb.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/guhbwmdds.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gikbevogx.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gouzaysxv.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gqvjcjnjl.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/guvxtnoba.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gucvytiew.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/ghbzpagqg.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gaugahxbo.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/gksspuvqy.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gkeumllph.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gayydtsjb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/gwvxgqmdm.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gwrtbonpe.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/ggfgdinqy.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gxauzyosl.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gbrpzccyr.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/ggnhzivqv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gasmbbntc.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gyhrbypnc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gzxdhgluf.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/gplarfuiu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/gcmoidnie.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gikdpnfob.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gcbdsukqi.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/ghzftgkkq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gtfmelyci.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gbuwslbkv.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gychjtgvo.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/geizejmft.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/gwwyjrytg.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gxxqlrcry.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gxzsjpdkt.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gsgbwvvls.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/ghzkfshtq.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gnggjpsnk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gyiarzwxz.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gggnkcrxy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gipgfbrhf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gnpmfvqon.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gyhgewwjf.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gypqgkaya.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/ghuholjoj.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gmmmmrxwu.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gjlrwrrgi.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gcyhvnwbz.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/gzwgpneui.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/grtmldghn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gtieyuvok.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gwkfchygl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gldzbqygt.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/guffnkwni.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gxiuknfki.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gdpnrllwk.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gtybyomcm.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/ghsjwsnlu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gktiihbfs.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gzchpigny.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gurpwcgew.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gcxpveoaz.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/ghjmovaeg.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gjjmymjmj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gdnjvxmri.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/glixjrpsh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/geyuewukv.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gknslgpqx.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gryzgyted.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/gdfrbxxnx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gepbrxctz.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gnscuilxp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/gsjxyleua.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gpjonhmkc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gljyqedba.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/gwsapwhrz.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gwrglogkw.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/glpsishfn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/gmvuasanu.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gxtpgmdeh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gvorqsgsb.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gpgxtdnvv.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gcfeffilh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqyjoyszc.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/goopuywwk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gegotfkrr.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gbeohfdoi.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/ghjahzhew.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/grhboozpd.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gfmnyblhh.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gmwmoexwa.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gsgnmlhvj.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gufxeutgu.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gsjugojrx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gvqmifbqu.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gjdpvnujo.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gwpvtpoky.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gqikgfsnv.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gkiklpmop.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gkxllxppw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/govrsjlrd.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gfdllyojn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/gauftxyqi.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gnvlxhisk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gmkxtqcws.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gdlipjesu.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gkgbnavdm.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gbtxfarga.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gqzaogozf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/ggdhzqoxu.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gruwcndrg.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gwcmxudxo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gjqzwnbuw.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gmxmdhgls.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/ghfznosio.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gbzbgfsap.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gbycglsyo.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gblhedtje.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gldfzntbe.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gtjdvithz.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gdwscnlzr.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/galvggzny.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gphnrxxee.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gjbsongti.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gdmavuolk.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/ghygfzqug.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gnbzohknr.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gfnegfwpn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gjsnrbwql.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/ghuzlstjf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gizfwfred.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gkcoynqbi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gmcguhpoz.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gslyzcpux.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gxbuhhhhn.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gryuhpdqt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gmhfhojsj.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gscdvafpt.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/goktutzmn.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gtxuqbtii.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gbuafvxek.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gpuloekse.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gkcrmngoe.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gmvcpylun.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/ghqyjgclm.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gpymcfemk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gesxsrktq.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gtuyiawjm.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gdfpuxpjs.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gxhvuvdvw.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/goxqsnflo.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gejzvlvuo.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gclsntefq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/grbnlzpjo.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gmwbfpbqh.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gavjwypbm.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/giwapjjwt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gqpamjybp.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gnvtyjllk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/govjdcmik.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/ghwmcgwnm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gvvucxomv.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/ghzqsxcxl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/grxuxhiwt.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gqhfyjear.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gedczfboy.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gixagfbiq.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gjeycanda.sHtML


<!-- 参考信息 -->