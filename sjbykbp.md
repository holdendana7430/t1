代发 wailian999

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzbztikm.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gvchfglud.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gevdyzusu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/glmeemxjk.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gnegteriu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgzbmuwm.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwmdopvg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gylapjtmx.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gzsckjtvu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gmshuwvtf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnubljfdc.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gzqeycfcz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyffyedue.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwchynom.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjucqjxll.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gesgtsztq.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfwrzlxq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhrkynjo.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgndnuor.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdqoeqqi.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gizmtcrrf.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghliodtil.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmflfxpe.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ginowjgkf.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gntmwkguw.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggolqwjgh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/geyzpvpkq.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gosrklbwx.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gilqtzpuh.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gcltaavat.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjburfvc.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grscikntv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/geuocuctq.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gqisndvtp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/ggrtjczlg.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/geedgaaea.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gupregqjk.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gacjlafcn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gplmszsoe.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gudmlkifg.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupbdiydx.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysbiidmb.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gieajbmao.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/giijheswg.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/galalzkpv.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/grypdzgib.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gauvkybas.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gwovfvkze.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxokydvc.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gopmcopir.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyicdmtp.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gccukijng.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqxqlntbf.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gjnyvjilb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gsmpygjpr.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzdvmclj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnucxcao.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbihethtm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gkarstzlz.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gjvlwijzo.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/grvmeltws.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/giwymeqot.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdibchlv.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gkarraalv.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gdhedyrnc.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvvpqzqc.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gxtrxszhd.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gtcazqoqc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gnpapfiys.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gjizaortv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gebmdjiuh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gywibltpo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjsutatg.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gylakulmh.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gredulrxp.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcvyzbap.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/ghixcludk.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjksbfylf.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/giqkhiyro.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxceqgkh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gtcdjpvul.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gjpyaqdet.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmomccma.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gtvsnfoof.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzmncrhat.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpugftcn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlkqargy.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkddzeoz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbvpcmft.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gjyjhtrol.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gfagxzaem.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwnurkax.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gteymiuce.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqiisjuf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsspieff.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gwmpanzng.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gzfnigqso.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gbfsslahc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gazchjgjg.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gaicwnsja.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/govknzobt.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtvfnbml.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/guyftzwew.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gesxkndwg.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgnchzth.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gikxyacav.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqhziaoz.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvbsckibp.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpturffu.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghchnzonn.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gilykngbt.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gcnjlmjjl.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gkzzkoorg.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyfyvisp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gurcjszgm.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqyqiwao.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gizkphqge.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtswkeup.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gaayxpnmy.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfzwpyhb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbhqhzgp.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gabytihnt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gsjvtligo.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gjgfzaknm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpzljedx.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqzggpkz.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gfemcvidt.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gipfousoi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gvoyfdzin.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gaibycutf.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfemgvxy.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/glrwsgfcj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gixwilayg.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/genhkiuql.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gtuavrlvu.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gydhrpzgl.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhpmpsxz.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/grlqtljmm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/geqcmadof.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnxtohba.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqiuknmk.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwiiuguo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmparmcz.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gsufjlaqo.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/grvyhlrjj.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjmnuikk.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gboxpfrwr.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gkwjbzkci.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gqgeiqobs.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/grglymzet.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbykhgvr.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhdgwwir.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjuswcsv.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gbtyjzwzx.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gmagqwblh.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gnsbfoyaq.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gkhppseqh.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnixunqs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gnutedamz.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfalxcxe.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gaaeiermo.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyjtzlib.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwtjrwwv.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggujhydxt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gffufyrsv.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/guaaaykpv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gzdkqxytx.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/ghajzhumu.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gnfgxpllu.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfzizvfq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gtbtycxhd.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhbmygsa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gsmaeveph.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcqfshhh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gbpopcukw.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gcwwlawrf.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamphxuog.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gpckmsiqh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/geqmpfokd.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gpzopvipk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/grtartysh.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gwtcmpdga.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gryyhxatv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gowpdpbjb.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtusnepz.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gebexjxxo.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/guoxnhixm.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gjpcclsxz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gugztzzso.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gslkqkhrq.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/glazotlzx.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gjlzmnfjk.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gtkrkdqga.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzsxbavn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gwrqguobd.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gekosqhne.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/ghpvxbbyk.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gkembakni.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmtuwcnw.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gkiebnybv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnvhirwy.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gjszzsnwb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gedofqnya.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrrdxfcz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/ggcajramk.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnhcaflh.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gywamqabo.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdboidvog.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkjyfgqy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdodfepps.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gucdaiqna.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/grkpeubyw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gwnregpys.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcxcdhzx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goulmancg.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gpwkpqnec.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gpvyxyhik.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfpfmiws.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gndkxltyv.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/grmkzstuz.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzepdikw.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gmifnbork.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmdnjckq.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gydjwqwfe.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gwqtaajma.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gyybtjden.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwjgxwnf.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbncnwfyd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnqtorwu.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gticzjnwo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gwnfynxch.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkcmkboo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvdasxgk.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/glalywwii.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gipnbtkuy.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqzqqqou.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsthwctr.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtbdudba.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbryaovun.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/goncawyer.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gryjdmiyv.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gxgqkvccb.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/giebqyvbo.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahweixhn.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmctowni.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwibqlbhn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gonpqltgs.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/ggshzalwk.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gylwadjnl.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqwnfist.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjftjyao.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcbhbmzj.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjrklkqh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyslxhqwv.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/glseozgex.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccafevog.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/geyepmaeo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykcslsba.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gkodfaxra.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/geebephgo.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgkotcpw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gephhyjtv.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gnahcgccr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/goohbhlpg.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzosetly.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghccwunbo.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gfvtjcelb.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruawohce.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/grlcomtuu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrzdgfde.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxoovmta.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghaztwkpm.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/guqmxxjnw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gbrmypbrc.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gcblhwzoz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxojevso.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtqavuhp.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrkfsfyb.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gjmwhejrl.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdrdnkfh.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gcsmttiua.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gtxonjisb.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgpdbqcj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjdqpfor.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/ggcfolqea.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkdrcdsc.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggosqjgkv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefwbvsbf.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvaqnxuln.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gprpuzuvj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyqsbikn.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsxbmpaa.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/grhgjhckr.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngyetwrj.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gefgmlkic.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/ghstygahk.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvyfxvwk.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gcpzqfdzd.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gudgaxafo.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaulusfly.sHtML


<!-- 参考信息 -->