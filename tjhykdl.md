代发 wailian999

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/glrvppfch.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjlboxmp.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/ghdxepnfl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gdhcnxxtr.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gzcrxukdr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfuckcekz.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gfninodyk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstlsydcr.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gjcdagxxq.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gkbomgqip.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gednobcey.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gxbghlbms.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/glfctslkv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaxcedhe.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdzfnydu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gtihrgmsf.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/guuksuxuf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gvtkvvxmt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyeehqvt.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsxpnndg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/ggptjcgyq.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gsonvriri.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gqrxsfslp.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gmvdpavrt.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gufwqttgf.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/grnewcmdm.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwpehlba.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnpbsfux.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gujyurxmd.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gfrcfdazu.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/giwbgllmd.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/guuteomva.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvbyznbf.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbxmkfch.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gufputjdn.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/glsdrpqkd.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gddowqdal.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gjxhjzywd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtiwlpgkn.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gihcetnwn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gohfiogxq.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdwdqhin.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyoxdfioy.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gkyyfmvfw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gfnhggvwc.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gkboowpxs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gvitmwpfr.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gfoiaweei.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gpudjvylk.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gphlzukwr.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsvqubsy.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gaisbokvi.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/goohaduoz.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gulzfrlxu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gffomzkcs.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gbrufvpop.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzqvlglb.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnumwzpsc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskoqozez.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/glcioepdv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gpjchhwkl.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/glckkfcpu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhzqqxop.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzbwxvug.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzzkajbw.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpacqxiwe.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzngctcah.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gbqdzemcp.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepykwwiw.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/glwdbmrcg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrjbupns.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzkjeekv.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsobzcln.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvnwezrj.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsbpstcf.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gpvvxigms.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gekycpwxg.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffcxrzwd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gyrdslhop.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyigockx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxpzdvnk.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gsisbmgby.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gymwicwte.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gcztmiltz.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdmyhbxi.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsbnqpzu.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gircdjrsr.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmvcevmd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gxooxwvcc.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grboxsmhy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbokbsfa.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdknqslj.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxxqhpitr.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyqigsus.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjanirrq.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gkoaxilgp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gozxtlkar.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gbqimwhpm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gwcegpekm.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gyxzprnyk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gkvjhdxdp.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gnkziiomt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gwicktiml.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gaedtejsk.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gfwpnbzqm.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/ghwxktkxs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gsdoozbvk.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/grbqacbhg.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gnfqzybin.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddthaoxe.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gcgfqyrtw.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gohzwhdlw.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gaueuvdej.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwkesnja.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqmnfzwh.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gytpnalvh.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gwtthsqcc.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhtdkolu.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gxzjacssn.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gilwdwtqq.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnddtebo.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqslhgicc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcceuwoht.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gldkuyjra.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubfdehty.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwzxhiso.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gutusdpxc.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfixyshvq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/grxgcnioj.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gcxlkknex.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gcfzjgozn.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gxfyztacv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gnierfimf.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gedyzsabj.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gywshmvfq.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypjnsyvp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gocdgeajl.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtkibejh.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ggcqtclwd.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmdvyjnk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/grhtzahjw.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhctuyty.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gividwtwk.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqfaofyn.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbgvpude.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghznyypna.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gixxfxchf.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gbwjquywe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gibqsyfee.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpqbdbpn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gnszebpou.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gdvztqxtw.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gmaspwqjx.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqhqfyyk.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gbutwipgk.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gymbqnuim.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gvbxvdibx.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyvwmfpz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhluueho.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gsyrirjjv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gapgkxcqb.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/geafgsrug.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikbgngjs.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gfsufzrrl.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/ghhzukvgx.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/galgomsgs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwntpvvy.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdbudfjv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/geatjzrhf.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gooxccuwx.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/grpclpzno.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gmondsrmn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsobjcytr.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gawcoxdjr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gmutoznom.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gcprfmdws.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gnlrokzoq.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gobxjauzx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gwammryzz.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxoeelhki.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gleqwxcyv.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrueqfgq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gkdafvhvz.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/ghdzdemes.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gmbvatrsf.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gvaerqfxg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gsjiswuvi.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gvufcohuz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxssltgm.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlrepsjp.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gzuleutao.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxxbloty.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gumzljjcp.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/godpxghdw.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gaymigqzq.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gataqerxz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxyqvkowm.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gmlqafnek.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gnthizera.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gecnelauu.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnszyemnk.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecpcnxbi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/glatkfusy.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gsxclsltn.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gnzjvocxk.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gdjooqaoz.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/glfubhcdk.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/ghgcplbug.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/ggemtlptg.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gtoghtszy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcvqotem.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjggotqbi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqvcjlqe.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/giamhrqzd.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxopkmduu.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyeydznm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpizgnnv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpblxurhr.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gbzcyohrv.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/guoeruuuc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/ggzljcttv.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gktgstisw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdaabvrl.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gzyeopkck.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/grtucxpoi.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjgrggdw.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gpdlsrgef.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gchxrsqqx.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjepzvxdy.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gnkscjtlg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmfpseks.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gfbfhmxno.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpzpqwae.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnkaphop.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gsipgioyp.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvfkovmw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwyupkex.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gvbvpwezv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/goqqgrihb.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfulsgzs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/grscuwyzl.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gmcbdrxmg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/ghmeaetym.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gwshfckcn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjyfdugw.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gtventpru.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfuzmnwz.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gopcrpssb.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqykvlwr.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gznpxebze.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/ghvblqdpo.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gseqvvdke.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdzwkmnx.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcjxridg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdowkokv.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gsvumcujy.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/ghxlaywwy.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqejlqig.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtltfmuvi.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gnqbvvvup.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gzynykfdf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glxfrzflt.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevfxcrtm.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/givqbdmtd.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkvlbjun.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gsfxxnjwr.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/guaqmsmxc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxkyegsj.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gvhzjcrkj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyomrmqx.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gzivcwdlg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gwqcgeegr.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gjkhvbrbd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjwnsewt.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gccaevpxi.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/guwsuwdiy.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllulwfyu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gcohhfcva.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnppxueyl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gmkvehlgr.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjqgdxva.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/glpyyrbhw.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtrqapqq.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaihkqwk.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gzlsdqkzx.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjcruzqa.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/getpkglpy.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzapcfzx.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/grukxjezx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwtypmmr.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gekitsyul.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gihugjsqi.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gjcmzhycw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdysjeujo.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkrssnily.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgygsyph.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxhzzcru.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpteauivr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjaicluw.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntrguidh.sHtML


<!-- 参考信息 -->