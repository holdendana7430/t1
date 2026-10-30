代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpurrupv.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/guauaivoi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/guucrdfmg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxeylhpf.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gjshvcruo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnbyvjqh.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gydxpnotd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/giqjtzpuu.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gaxqinbtp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxnejdbz.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/garoyudow.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gcswxvpxh.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/guzsydfhw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnukjihoj.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gywdknibj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gdrqnkzkf.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/giytbwinl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcktjltdk.sHtML

[Q83] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gvemcsbuy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gamuhvotu.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gftfytiao.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gicnycbgl.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpuduscg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/glpdcjbcg.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gdzxgdmmv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gvmswadbg.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gecobqbzs.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gbmjmoldu.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/guwrlgqlu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gjspwfemf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gepgfzivp.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gtaherhoz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvetsrjcw.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gehiqexrb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/grkveucdv.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/giqbfrvgi.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/glegpbgzn.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gthcnrhap.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/guygkbrxx.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gbgolohej.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzemmurmz.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyxksbwo.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyznanxqp.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/guipdqqrn.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gnwlhugaq.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gddrprhtb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gvizndqcs.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmsqsasi.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzbotatm.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gluozxjsi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gekuvqcql.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdxvcllbe.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/geipdyfqv.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gztnvyovl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gllkhkrxg.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudzyltxb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gcdzfvhpw.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwcvpjbc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbxjaeny.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/grxgmbwfi.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gjpfbhhoe.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmgcjhhw.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gflldfznk.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqxprctj.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/glvzgilfn.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzicrdtle.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjmkjbqb.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvggkxjq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gtwmcwaqs.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gewfivoou.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gmwlzvewl.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gtywyfusv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcvqisvb.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnexsgzy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrfbtiom.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkcoczus.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gwhrovasd.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gqqpexrff.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gzpdfqgtv.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gdxxlvfxu.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxxxxwya.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtppsbua.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/grjtaivqu.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gfywbqkig.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgvbkola.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gcxwzfvfj.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwdlgelr.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmgehfiy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gzekkpwtz.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/grronlygc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gyqormgcb.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzkmqguf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwppmncwf.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gckibksoo.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gfhkdpogt.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrnziehj.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzxowxnu.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/geslsxqtv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtyqtwtc.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsgxhubl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gyibzntov.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gxgvmzlzt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gexjrledg.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gnsxjvyco.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsstbfzs.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/glhgbbjda.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulkpfbiy.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gezvjaivt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gyjbceesf.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gckfukqsw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdjthvlu.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gncmuztuw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksbnmcbm.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gofificae.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjijilgi.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gbytpcumj.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhvthojp.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gbfsnrhvk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gwduhjlnt.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/grhmpbvok.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gvigbwowt.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkkyeulr.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwufmtui.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/girlwhxow.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaihzqtcc.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gwxczrkab.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvdgyetv.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpxnslrky.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gvwaglerv.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygzxlbnh.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkhpqoea.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gbzsevttv.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvraolmi.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gthowuitc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gnxyjfpzb.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdzuifmw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gksxytobl.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gfsjorilt.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gveulurqz.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gppetwyfl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gvurbcidc.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gvrfajpnh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/geyinvmzz.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gjacosuhf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzpbyygv.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gtapxwfuq.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmbfohio.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gsaxkkugz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gusmxwjoo.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuvdxvjq.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvwlulcx.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkanqetuf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxyoxkwo.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmcnwowp.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gqnnrfnka.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/grsgxnkth.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnjhmffc.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gucxkfukf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqllrxib.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvkqzsyz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gfdguvrhv.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/geeoxodrs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gpryksqyv.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrtefxqr.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbstwbizi.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/giissopum.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gmygsydhq.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpoaakjc.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/glqddnwrs.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gyrxarktc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gmluyzfjw.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gvtqlubej.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucssckfu.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gjiuwlkse.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/geqncnrpy.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/glasagfdj.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlqqsunq.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqrkbnif.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/giizdzvxz.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gcoakpawn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjbhlacl.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gsdmsjiwa.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gdilfcudb.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gsuecrqjr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gdrovrwal.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/grsuriihz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gmzgwxmlf.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnvohwoe.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gqesnxwtm.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqfyhwkh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gxaywxpuc.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhyexhmb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgegchlw.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlpepfoj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/grckkufpe.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbcffkav.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gxogumogj.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzwrbvhs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjsahnbm.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gkfxldbpt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfdjqcfm.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gvrzjqaqx.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/grhpzwycx.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghevmhugm.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gjbxtuzjo.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/giowvhmvy.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gazhtdibn.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrejvred.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gadwgicib.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxvjvcao.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbhjnmtm.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnevrqatk.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gxobsfztk.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuurvhci.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvuatvxr.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gqpjvnsxw.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfakgwhy.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gubauqrvs.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqvpuueh.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gbmstmnmq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/getknvctw.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusveehzw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/glknwoztd.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjeldwdz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gcndkkefj.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpoozymh.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpimpodk.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/giuzrnmhx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpuaksfe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gznygjruf.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geumvubmo.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqjqqeymk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghohrbgot.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gejbbgzuv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtpzcjyd.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuibwfzb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/glrvtztxi.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gxblqdcyb.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnuhytjp.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvwrowau.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkrnfeoi.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkudkjft.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gqhfmipbc.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gwkleszod.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjyhvrpr.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glquersdu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuahwmna.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glalfkgyw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gklqtljid.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gylkagwcs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gazbnezdl.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjuokqnn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gxlnhiqwo.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqffbobt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/grhvukxqb.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypmwtvrc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gwrzwlxxp.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/glplfvczn.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gdsfwpwhv.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gwppdlxcx.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gygrsthif.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllrzncod.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gxgmbyhur.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtymxryiw.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gqjxhhzzv.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gqtisknpp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/guitknrsl.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gedsloodn.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gwfomvdqh.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gklkanldt.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gjneanotp.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgjslrid.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfymfjpr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwbrblte.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuvkdfmo.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlhzwlai.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gxwksgolk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/glkjvwmfx.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gubrdsgza.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gumlslpiv.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gyhebzvrl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeletmbb.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdikwlam.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/grybprxaq.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpvnnexr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtziqrkgk.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdjgtoru.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccsbrynh.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/giuffcaen.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrjkqtri.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gccuvqjfn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcjncbql.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopaybeat.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/grgbwfqzc.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gputduhzz.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdxjzyqg.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/greqmebtt.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gfdjghxsh.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gabjpnpxv.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gygfklhjm.sHtML


<!-- 参考信息 -->