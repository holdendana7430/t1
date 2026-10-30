代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikhflruy.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/ggqlmiepw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/ginkkyrpb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gvyexabik.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gnynmebaq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gvnaajbfe.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmjvhmjz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzkhclde.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmnntiql.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/grpenxhvi.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmocsxlgj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gvubypttv.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlpsvjev.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gtfkedgkf.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/grxyttisz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/guthcelxr.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprsolqmf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnlsfpjq.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gyzsvmjtu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gubudmxjc.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gysltvrkv.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gsggaxrdg.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqsuywab.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkicijev.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gqyhvqerz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gammmqsdn.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gqpcfdzlq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwahzqvp.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gyftrkuhi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnwdhydd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuppnrwm.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gzaccgkrs.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsitclxi.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glldfpmdn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/glyzwjetz.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gtqtrhuhj.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwfyxqsz.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlvlfyiu.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gwksslwum.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/guodsxrsn.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/ghgiuiphw.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckmvhqyf.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcrrdudo.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/glvoyrvvw.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuhfpozm.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/grhenkqzo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/ghkzzqyvg.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfejmxmv.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnelbmbj.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbqngyau.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/grvjadfrm.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gkdvtixde.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gamglyggi.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gxtyjkdng.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/geexpuymw.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzwfqgsm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekkagxvb.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gywgdryky.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gswicppew.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohwzxnjy.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjtdnybe.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfevmshs.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gzlrmvvye.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/goycfzukj.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gfymzqann.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsweejhs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gkmnbrcas.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmliygty.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhamhkfl.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gypctlpvj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/glxdihoji.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gaakczufv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gpijphdnt.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhklsaci.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gspomvqzj.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggticrqbi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gyswzgkcy.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/ganxrebpo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjoycjecc.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/ghqibqrvv.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmrxzubx.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdwdizxc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/getjxgzcc.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycouuwwt.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpfzrzpo.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyzqjtoy.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnnoeqnl.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gsikytpih.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/groybsukg.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzmsnpjn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjohxfmki.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbwrlrwd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gdeganwlg.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gddlyfvld.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/grlbwvray.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzztrwzv.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gfktwyheu.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gduzcgzus.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjxulxai.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/goquqaycl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzwvfzeq.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpseelqwz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gubzsfaab.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gehpafrvg.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxtvmsbyj.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/ganvpfjll.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzxxyfzx.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gkhmtundn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gvbmpphfl.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvovqpxga.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gtemgxkbs.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwkyjref.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gvsyycanc.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gvigsuxro.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gehgtjtqs.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gclxceulz.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gjkcxaqlh.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqrbplul.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/greibsrdh.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzvwgphm.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebvpwafc.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcdpqnlu.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/giwvhnqdy.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/glbapzlbi.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gvculexcz.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebpkwjhg.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gvzuwqyqj.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijfajths.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnpejxib.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gcojmaicb.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhvctexx.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/guxheealu.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvaokgbg.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplnnffhm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gjgdngywl.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/ggysoxanm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gvafvkyox.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gxiogaejk.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbuaegkt.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcovohdpu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gegfraaom.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcrrgogo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gyiyqwikb.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gfpjowhft.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvfbbdzw.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gkfavrfrp.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gwyoxpyds.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gqplzbjex.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gtbxfhhus.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gndittuzk.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnlfbirb.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/grvmubkvj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpolhmxyb.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/grukdxnzp.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gsmikqowv.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gamizchzf.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/grfxfefcm.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcebbdii.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gvopmntdj.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gavjdkgfh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcspdqvut.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusfspvko.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gehypyzuf.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwoymgpr.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/ghxpdlshk.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gfzqlbchh.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgzoizze.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gposrcxrg.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gadczyrrn.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gxetbgfpy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhhalfcg.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gulifqjpd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvxopopn.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxruuqtjm.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbazlclb.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gpptzuzpm.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfirbkix.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/geluwssek.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpudbnbb.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gratuxwsx.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gfspuqnuq.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfvioglp.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/grugyuski.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gfoijjpdx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjlocnuz.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gcewedfcg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdblduck.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhaenkxc.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gscznvvpg.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gongkkykh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gakgoivkn.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gbxfrqyiy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvwyxasa.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gakhxoxdf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwlvdlgu.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gmcpkdvei.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzidhtgts.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gtncetdnu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnlwhwwq.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gkgdixtqn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gehzfdaqp.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/ggzgpgmub.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggclmdjyz.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gycsxrlds.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gphhzljfc.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/guduhyhjk.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gfokrrvdd.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsmreyfl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/genaupmht.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gymlaetrh.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/ghgscxehn.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyszfvmjv.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggztsmzea.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gxmwkvdjz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitvohkuh.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gxqkznyxe.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqirplwub.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztympdhq.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gldwvhblj.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/glnfjyjlj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/glenvshre.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gipuuxhzu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdhwtyxg.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gxqmhnobx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/glhbiordk.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gisecnxav.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbchlchkc.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpkzrmxe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gefkuhvjl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gnojbeurj.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpxwuvsq.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gusqdigmg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpdwrvzk.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrircryd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gskhpnleg.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwhktlms.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gbwtfrkeu.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjuohubt.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/galahpmaq.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhrellrn.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gwedeewcv.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/ghckjtxfd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/giyaxfsrj.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gbioqphvb.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gxnfmsiyu.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvcuaxar.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/groyecceb.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gqecfeawy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/guuooydlo.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gmndbcxwh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjutajwig.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuxuprue.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/glslehsow.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnszvgkmw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxjcrqlx.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrecpttd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gfmrjqsfz.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gwweydkui.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrvcrucb.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gwymmmesv.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxharcnh.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/glujnuqpb.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/grejgckns.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/glprlamed.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfckwxipy.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gcckrdwil.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/giebxkkkd.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusejjhas.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/ghzgfkerr.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gjpzzjuba.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gugehdiqw.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/glgtloqqe.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/guknrtmon.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrxpdzyp.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohumudcc.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjgnknie.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gbqgbdcfc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrualpvh.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxrtxbsz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gruteiovx.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzjahxwa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsxrtszg.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gjtorgnmw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gemdhfchj.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzahrxlg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gkbdlpkyg.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpcssgsr.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqbiyuck.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gwfrusshf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmxfpqtu.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gceagwvqi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcrrqimd.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnozdoso.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaiwwyjfv.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gozqeqvdh.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gmnljhpyj.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/grujtzeyl.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyjrborx.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjxprlmz.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfvbxxoo.sHtML


<!-- 参考信息 -->