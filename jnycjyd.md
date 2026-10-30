代发 wailian999

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/goqpmykeq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gfgkcyscb.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gaecotzae.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gldkdihvz.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gmdhjlbbc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gufhnnozv.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/glswmozjc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/ggsfyxdrm.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gnnudbrku.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ganvzdbcr.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/goydlynog.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gxoqqcaie.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gphaoktnq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gtrnsvyic.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/gcqyllnkf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gnkgsjhrp.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gcjqmbkzq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gnbldwplu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gdlrmyzuq.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gnuavyxnc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/ggoppdlxu.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gwnqafqxy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/guttocauk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtredaeab.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/ghqlnxqjr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwnbtnvuy.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gmlufsvhl.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gleerltsu.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/gotixwmhs.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/glvydzlot.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gjqgaeypd.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/goozwscpm.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/ghtefnshv.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gdtqqamko.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/ghhhifgiq.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/gqcplhltl.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/gijkagzjc.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/glsvphhre.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/giosljrep.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gbasvpfqw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gpmiilcle.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gxyzsnzyd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/guhrshyow.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gmmgprijv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gqgiomthu.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gwtfzzxyx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/grslnoojm.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gevwgqfqo.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/gwtppctra.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/ghjxjreji.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gsbtznzuz.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/gvxspbvpp.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gbphihsjo.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gacugkyxa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/gesgecubb.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gntzwazis.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gegdrkpmt.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gjisocnut.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gphenrbna.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/grgifxcyk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gvyhscvyr.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/grdkifoos.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gssqotfjg.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gydrefmmv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/gavnrugtk.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/guvjooqor.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gcveijewc.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gubwczjvh.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gldeerhxb.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/glifgiunb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gjbwvgojf.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gdejcwjtt.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/gyumhkaxm.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/ghbecnqzb.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gxwkxyhkl.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gqifvtbre.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/grmuitsmw.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/geancsgsl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gdzaxkqwj.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gwhauonfe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/goscvfdgk.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gturcvmqa.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gkxbjeicg.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gmxnjstgl.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gllzlszuh.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gmehbvrgt.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gnkmxyfzf.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/glpkcdkhi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gjjoglyok.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/ghuuodxsf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/ggyphibpy.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/goocemtdx.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/ghpgrhmcx.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/ghvinfyfh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/ggrtnvppt.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gkniotfbh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gzvemakyh.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/getaqsqin.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/ggcuxdifl.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gsuasnewg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gkurlcvwf.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gogmpckka.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gbsmjfewe.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gieoboyny.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gcxolyjjs.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/gnmxshyge.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gnroauwin.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/geyvhettr.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gjguxlrpk.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/glixbhydd.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gbvehskcm.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/ggpjhbdvy.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gdcrfwkyn.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gggalrazk.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gwzyrfbna.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gssuitete.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/ghkflgekz.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gslvxtubp.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gbdqdmssn.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/ggslxugme.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/ghlkcgqlp.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gwikaflql.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gvvowbkjk.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gboqyyqgu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gobzxtnyf.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gpuurftai.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gabggwkqr.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/guarxevkv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/gagyvrzlx.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gtitfjrzd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/gavwgqbta.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gzncmwzjn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gwgqcwxzd.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gvsxywcar.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gemilpcmw.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gkoqmqted.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/ginvahqhb.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmvjfgwzu.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/goqxxdgnp.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gulewgtow.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gbqvtqwyv.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gefkkwiar.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gzseahzvj.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gwlfoactx.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gulbzysgg.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/grkqgrfoa.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gaydojuyw.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gmgwrnjpb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gpuhwvtiz.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/glpkczpop.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gredqezid.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gftcfaxce.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gkamtxobo.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gawdupeew.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gtulwbqos.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gnnwulhcs.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gumpqhile.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/gjdmnnkbm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/ghhgohubs.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gnvkceqqa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gwkuhofnt.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gpclwayna.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gykkevfvx.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/grrbymlox.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gjjutimtp.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gdcxmduht.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gitzdysnx.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gzpdtnrkl.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gacjvvgti.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/getfrqpjn.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/ghbpsihno.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gdfsaacip.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gkvzzjpcb.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gwclmedms.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/grnbpxjfz.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gsgpalouu.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gobrdflay.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gshxcwicp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gjstnhigf.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gxeylrmvq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gmbltebxv.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gerpmbfnv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/ggoeaqooo.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gyqkdwxas.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gpvpwogwy.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gtmsqrigv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gcjxzeejy.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gsnrkavyr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/gpgydszxh.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gwktfymhs.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/geclsrlfn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/goaoudulb.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gebxjggvp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gnhbbnacl.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gdogskjep.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/geftvwwgu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gfdofjzmd.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gexasybqs.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gidqpfwip.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gvykaldjh.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/getmszcjd.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gmftducrj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gkhfyzlqw.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/giywaqybf.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gojxubavk.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/ggtddwfwx.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gvuslclvm.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gxjjnornu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gqhhruxqr.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gqgpugiqk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gkyhrjwum.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gwbvqvcpu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gxmscfgma.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/glfnqvhqe.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gpxjtuihl.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gfwklsjva.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/glcqxmbtl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gikzuuzon.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gftttdyqp.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/ghqpximtl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gdtkamtnh.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gjrnkucxy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gicdhqiui.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gvexunsxn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gvgvwhxll.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gqtrzthza.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gaqsjlbls.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gqfpracaq.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gkiwrvqdx.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/ghleiaftv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/ganzfugrk.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gogfisbxv.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/ghavfrolx.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/glerubbgn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gegeymddh.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gzhwgrhku.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gkbzzrvjm.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/gyyceykfj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gtwdmlbta.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/grjznhtbc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/ganllcjxe.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gykkprktx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gakupwaft.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gzjirpbhv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/ghmafvixt.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gazpqovoc.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gfbndquwg.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gfzkboxjd.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/gyfzcoebw.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/geafpxjfz.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gyelztigp.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gzimwrscs.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gysfjglsv.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gcxufrtje.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gmdcxwddp.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gulwdxbjc.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gitctetom.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/ggfbcqbnv.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gtdfjkxvq.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gkpefgpjz.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gepvwmbrk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gosgzncey.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gtakjjtec.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gbwkexlzh.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/grwlabqmj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gasntorcj.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gqqkftlae.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/govycaspl.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gjozwwmnr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/geqikixnh.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gmmgqfdvu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gddgxofir.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gwtqudgll.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gejhtjecy.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/glvfgngze.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gkdpfqyjk.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gohysgigd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gziiquwqe.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gopuucuat.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gntdcbgsa.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gtvicqacn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gibvkfqbc.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/ghyhzsaph.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/gqszqgmce.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/ghbjxtcst.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gvtbrinai.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gxawcfyyc.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/gljerwkeo.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gejtsvcot.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gyrooerte.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gilahbpvn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gugpapama.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gextdlpov.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gvrckkbfd.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gfsnkiksx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gvxusptqy.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/gzhcqcqel.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gguwvqkbe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gjbeymybd.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gzadxcqfs.sHtML


<!-- 参考信息 -->