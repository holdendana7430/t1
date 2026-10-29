代发 wailian999

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/gxnfqjhpv.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/goungixzr.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/ggvnbgkwk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gavuicuax.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gqxwicbpb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gbogsjeul.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gelfppkiq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gsaulijil.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gcdhouiap.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gjmnfyzpj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gadkprqls.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/gmizzmnfu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gssbzwxit.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gdvkevmtd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gmavwxhqs.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcpspnhbo.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/gexzcmvkq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gooyjwrot.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/goipbljxg.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gowxojenh.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gvnwekkwb.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gkxtlewvz.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/gfznxrtwn.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gffzyoynt.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gifokpazo.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gheqijpxt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gogewhpgj.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gddyducjv.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gdqhbjoip.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gwhhfvmzg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/ghettgvav.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gurgkeaoh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/gzvjzlpie.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gqxdvynvf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gouonvpss.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gyvdezidd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/giaitrsle.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/gjvtldpbs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gqshxbhyg.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gjwwvmtui.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gnwlaotaa.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gxhpduwkh.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gkkehmdjk.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gtfdkjcdl.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gyqzztpgp.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/glbvqwojv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gfvfbhtsl.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gvzvmanqo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gwostbocr.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gcuzbgmoe.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gkyyxmiak.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/goufwzbsz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/gpnlgvsih.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gpampdpxd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gsvyfdamf.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gkxeqcbvf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/govrrtdnd.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gifakjngz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gagavjorr.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gnbflzpbl.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gkmhskksa.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gwjnntdpt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/geikejzdh.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gevnrhumj.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/gegtcwwkq.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gowgxwwql.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gtuxarxui.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gkmggdiyq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gcznarcqa.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gspgfonnv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/ghocbqruo.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gvbihvhyv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/glacauoyl.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gwmmjmiia.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/galorlwmv.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/gjnpfleje.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gbkbcdrnm.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gcjxpumgg.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gshuvmttz.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gsvxarmgb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gjzbhguxx.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gjrkhjmps.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gejznndvn.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gxhqyzsss.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/grkgfsing.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/gemicwlrg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/grhxrhvzv.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.hesvh.cn/Article/details/gfuoavlhp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gbgwyiifv.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gppvhpkgv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gqvdgpssu.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gslzkcseb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gzvvjoxti.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gahnjgwpg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gprndlnbj.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gmycvgckw.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gpfrordde.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gczxenpaz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gobnyruyf.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/gvvrdoyej.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gdzdqjzri.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/gxlnmfluz.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gevlinglq.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/gdrdfgxux.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gqzmybqmn.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gdmsjiioy.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gqlfvfapr.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gshxbrjtb.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gyrxmqkmq.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/glibfjwoa.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gpwjzjtsn.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/gqsbrknjb.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gbafdpxnf.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gnaxfhpno.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gecbtphpx.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gazucmozr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gjlcvzjvr.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gzaalbexp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gqindcosk.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gwyvuuisn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gnuftgjay.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gnflcgtzv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/giexamfif.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gsvhppusp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/gvvmolusi.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/guufuixco.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gbbzyweaw.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gocnjmvhp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gnnhhvsgb.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gmnprkrxm.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/govbhzuqr.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gzesggqus.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/gqhkjmqhq.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/grlqdwymp.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gidgdlwwj.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/gtwhlvydx.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/grvmitjjk.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/grozsnluh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/ggkjntxcb.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gvrqnylks.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gmnripfwo.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/ghgwuoryu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/guqyamtkf.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gxbknuplo.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/glyczjjmt.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gfbypffwc.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/gmvxmqsoj.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/ghlaqwewt.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gyxbkpeyb.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gcdphwjub.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gozbtmpfe.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gwkjyszns.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/ghwrdlzfp.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/givhqubat.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/gruatdfec.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/gsofetmzp.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gzstpwykg.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gefseobyz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gelbprniu.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gregfmurj.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gydvsrdhu.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/ghimanezr.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/gbfdiqjvf.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/griizbcec.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gloykifkc.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gysjvnoow.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gxfpldssc.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gevicnrcu.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/gbcvfjbbd.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gexyrypog.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gcyeaxdiy.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gfsowhodt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gtzipaubq.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gkduswfxa.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/ghhosoxql.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/glktrmqwf.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/ghezqmvcs.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gufcbfcyq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gmcmcwqqw.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/ghijorrnk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gfevaemag.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gngzornyz.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/grgogknuu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grupnczox.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gpzhwppol.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcidzocft.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gvbfuszzm.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gzcogrtuf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gbvydcfts.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gsdvuzeej.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gfgefufvl.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gxabjxtvc.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gephpyyfb.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gkbzjpqsv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gwcxndlli.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gilkhyzky.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gfiorwxwg.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gibtygykj.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gcvofhprj.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gfecptnxk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gdumysatb.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/ghasjbyox.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/giqasuyhw.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gsuyhskgh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gyqfzhmdk.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gehoofkpn.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gpbmnoeph.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gnkhamiqv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/gyxvljyvf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gaskardms.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gbchgkzws.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gtsuumeen.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gzacxytip.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gecbgbfat.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/goothqalj.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gqxtudzoc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gypgwthrv.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gkkhcfvyn.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/govbxjblv.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gyiscazrl.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gqhsanbji.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gyjmqyjbq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gdmqaphii.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/gcvzjhnah.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/giswasgce.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/gcfmxunhl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/ghdzubppl.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gxdsvdcbp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gfprkkaby.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gewhdhntl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/goxrjncsk.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gaeglwiur.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gwcbojona.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/goqympxmf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gphpkdsxh.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gzgxiqeku.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gbvslaqcz.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gqvfqhnwg.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gdfktzgqq.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/gvrrgpuez.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gepvvznyd.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gfnjrclug.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gcqrxekjf.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/ghrkljnai.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gjpzqypkx.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gddwesmzb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gysjppsmh.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gcottadht.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gmuqmpukc.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gafvfrict.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gpytmnuwt.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gxkqfuoon.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gnnfsllxc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/grdtmngpn.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ghpjlbjll.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gawiwsnts.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gpxkibxcf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gawwbqcix.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gwewphoqr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gnxlrsodu.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/ggahkzvek.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/glbpsqivp.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gltiwpqvx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/grpbfrqqg.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/goufnbyql.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gwgdihigq.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gbwlzemcs.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/ggitmnvhz.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/golxgzllv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gkxpxxdar.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gddjifjkk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gazryzzfx.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gcttapxbv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/gsiotvtll.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/gnvurapoq.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gzfsnsxnj.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/golgvbggz.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gmtzpaukf.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gdjrozznj.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/geididnfm.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gxxpizein.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/ghrdwbeiq.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/grwatxolk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/goweypgoo.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gykzohosn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gkupjbboc.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gsqqrtxag.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gikpjhskn.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/ghwsnzfom.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/giqwoqnux.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gmhvqlavc.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gklhvlton.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gktruddkk.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gkovcfatk.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gmutbifht.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gyhlvtisw.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjddglnjl.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/ghqevsdur.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gmyhtuekk.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/ggkacknbr.sHtML


<!-- 参考信息 -->