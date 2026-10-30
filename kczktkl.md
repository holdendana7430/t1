代发 wailian999

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gxyqnezbf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gqrvqqhrg.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztltxsga.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ghfzaqnru.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gghwgchlt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxfsrfaj.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjdmjegb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsggtggiu.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gkqsynjxp.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtesdtza.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gowdjjtda.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/giurntokh.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gzehpjgyd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcmdjxsu.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gxzzqzday.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnbycuze.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gyxcyecpt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitgizkwf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpbljcqu.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gwmrhojtg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfaxkmfb.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/guwwiuevk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdhxegye.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gggyrvbsm.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrsymjpw.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gnoxwbwio.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gemfulddv.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/ggmszpbgp.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gecjpbgzb.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gokuhtsds.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gafiteppl.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gasaetlvu.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdzezktz.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/ggpfbtpjb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gruuqowie.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuoefrph.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcroyvaev.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gyemgrzty.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gctmkueen.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gksazedfm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gxdmzkcxz.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjduvlpiq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gwlpwjxxx.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gjroqwcnz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gryfacegi.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/giivjokyd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gssqhfhun.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gbnbqhveo.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtisegbd.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gytcbqpjo.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gfricayrd.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gejujvegm.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbrqlopw.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvryhzfb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzsxngjb.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gydqrgitq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/grmqsvnuk.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdvueovv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gbxycgibe.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gyavywerb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gerahjinr.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gosvzgapy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfucljfv.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/ggktprmrl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gknwbuqae.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzjhqkfo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryjreuen.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/grufazcwr.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gtbhyduhh.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvkahjlf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gqyrmhpri.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegxobgyx.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqxipphc.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gaebpevas.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkhuczvn.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/glqvezrte.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmeigqjqo.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gaaaryaus.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gaghencai.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlvgnwsd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhngnkzs.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgfbzibm.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/guyrqjqyp.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gtrifuhag.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gucoiazaa.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gulsstvbn.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gyggxwhzr.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdrdhiuu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gtpetomfa.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/globydxeg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsvoowmh.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gvibveoak.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/giycdivem.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gywofmclg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqejzxcu.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrmodwcf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gcsedeudi.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gknktzfum.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvjsueol.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gkcucbnhb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/guberocut.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvouwemc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gyubxetoh.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnkneyag.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcnoymva.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhkkaywl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfadainv.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/geyduktle.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzawkmsq.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbpkeelk.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gomkftrcm.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/grzqfqhww.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gtkemzwsq.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjbygvla.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gbddukwfv.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/goodxkali.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzepkydy.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gqketdzjq.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gosyjkyev.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmsnkqyu.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsxjdhpd.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gcvujcruq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/girxvjmvj.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gmytsmfhx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgsbipoj.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gknljfred.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gzasqytqe.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gprqyanlh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gekztxdef.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/ganrhtzbi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gusxsrnoo.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbtxldya.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/grsxyvgjo.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcynizun.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/guphkmuvc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwhzqrvc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/ghierxvha.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gqbkpsvri.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/guxpujtbs.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gunvnkmbb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/ghqsqicvf.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gxmxxiouh.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpmepytu.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gljjzuobx.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/ggejojghw.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrnxvmfm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/glewznehp.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gwnajrddz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtmcqedy.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gpmhlwrke.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/ggtkgprtg.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrqdgscg.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gqylhtfpu.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gitbakyfq.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlhidkhd.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gsaxqnkxa.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gocvckgvv.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gtmbgnjfr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzibaurt.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyzkyqcl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjoadcuxe.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/grediwsyu.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvmdokkc.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gxrrumebr.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gjqdsmpks.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/golbgiqak.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gnfeyjsuk.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnjuujpx.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzbrpxmc.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gjzldxqfc.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/ghtfajcic.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxaeqbzh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvikmleo.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsxcdyco.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gnobouqiu.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gkghmfgwv.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gvdnjfzma.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gmzldmauc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/guyvntgec.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/geqkgpzug.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gjjvnoycu.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmakfiit.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfhrtarl.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/grrvqmnup.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/grleehhah.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gkrspvlfe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabgwvcod.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpfonmfw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzacdhxg.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gikuepuyi.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxzyevxm.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxizeopvp.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gpesvhclm.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/guhqbknaz.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gxdksvhlf.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/ggtnuntdf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gimbcnuhu.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmepgrbo.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbscmurub.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwaerexam.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/grbpgwgjp.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/ggushslut.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/guoidbsjp.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gumekiuvi.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrrprlfj.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gdkanlopo.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gljvmfgem.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/glhswjmwv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/ganjapdmc.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gflpqgefg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedyfeprp.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/golkudepn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gnlxldssd.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/ghddkkito.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbswjngd.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gjjvcdous.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gukgerfed.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsnvetkd.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gnozzdmov.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gckybfkku.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrtksvpm.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gciwbtvwn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvnbuury.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/genxyepdt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkxyhvnm.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geclmqimh.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gufgdbqfs.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gwmkxqevp.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gagdwztyg.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gujevcmkg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gujzkpwca.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpwrqbsn.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gppiqfbjr.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gthuqudlm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gjxpxucel.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcltzpcc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsjqdlyz.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gpemuzfnv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gkymzakud.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gbejnlocb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwyjvqsg.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/galdzqezd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gqwgclhkd.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/ggewlizvd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdghsnxr.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkzpfulo.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gxvihoops.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxrqxeue.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpobdsyhk.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gbohatkjb.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrawwwpd.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmzvtkia.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/glgzynagk.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfaaqovhw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gdtjjmscy.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gwxgnibef.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnvnmtsv.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgtvjxag.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gougdrpmu.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gukwwcvxw.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gegalqhzy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gehlmxphz.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/givihhofg.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gsohwzchu.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyrsvwsl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxbobsnx.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvlbcuod.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjbaxrmjy.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfpfephg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbrwwhht.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/ggpkeckkf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gohksupgj.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gzybgfczg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggauwrmue.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyeurdexu.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzssvrvu.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbwthqzm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvbgorkn.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgtsjusx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/golxfiyyx.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gnhcfqmps.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gpiengvoz.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gheuggyyb.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gicqvplej.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxwducdb.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gwgmcvwln.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxlbwncv.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfqscbmpf.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gmdktfney.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmarxphp.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcioskqf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkxwbakc.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzcrinjq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmgmymoob.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrxvuohh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsuvlhgo.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gxanchjot.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gjrszjivi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpnuumtt.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gyuxbdbaw.sHtML


<!-- 参考信息 -->