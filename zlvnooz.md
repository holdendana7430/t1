代发 wailian999

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gwkqahrgx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gtrtvsvnj.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gsnncdjvg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gygefqwet.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/grvgfsxrl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/guedfgdvz.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/glhnmzzej.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gvuenhasb.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gdzuciynb.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/glrkwmmgw.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/gorobdflh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gbiohfdof.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gxcklnibw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gnxxaadjz.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gzpxfkjjw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/gyyampwnh.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/gzfskjsqk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/ghzwlwnyj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gcwlbddlb.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gmqvjdyqq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gdostihas.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gsambnuib.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gfywpwzrb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvkivjjkp.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gixsmpkvf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glkgviirx.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/gsttnisyh.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/grnoskojo.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gksanpkcv.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gfrynkluv.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/gdvtxrikv.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gbsihqhdr.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gqwjmphvn.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gxwxlxudr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/gqtazjlsl.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gbxazfwmg.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/ggnhfknio.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/ggcxdouri.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gnevsiacy.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gtqudhdwc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gtnhjuiwe.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/grcvpdljc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/gngxzoscc.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/girbrvvnj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gvtnhxrux.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gtuwjyuzx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/gvtlenmsh.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gxvqwvrmq.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/gocwxcywo.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gpeelwxdi.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gpfufsrrr.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/gkoxvkqnb.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/gwztzurmi.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/gqduitmnh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gvzfvvvvn.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gficaucbu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gjhcxsczz.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gdfhywurv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gliqfuqzx.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gvnzodpel.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gmekpvlph.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gfecpzrnd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/glslkrndv.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/gbhjfebiy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/guqoslepm.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gsdvkpnwk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gmrskttpg.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/giquguuxq.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gastgazlw.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gyxfuiqdu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gvrwxqydm.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gklvfxtmu.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gfnpwikiq.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/gmfvwqjpk.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gglozljjj.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gjbzjwekc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gctsykghu.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gocgfccyr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gprdzcazl.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gdvmvvluy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/gjbtvjhio.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/gamrzjqgf.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/ggwbeomxh.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/grlulycsb.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gqdefclkm.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gyjumagkp.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/goakfvbob.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gguexcjie.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gfqohaxbl.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gkbfexhtq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gurhtqgxa.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/ggdydafzx.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gdwkihbzx.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gtqalhfdt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gnqazouvz.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gwaoaarho.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/gqohdqrxg.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gzkcrwfqp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gooxjddbt.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/grnqjtrll.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gmnjmpfcq.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/ganpggjay.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gtalvuzlg.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/gwyjcqzgx.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gyalpabqq.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gjrdwtyul.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gwpmysjzx.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gtieyvtsc.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gxelthsxa.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gvndnjkuz.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/geoffzfvb.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gljgjbzci.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gboacbpua.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gtawfhyro.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gvwocbfap.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gxghlhiia.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gxedagrbp.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gycavgqzt.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gfgasbtcl.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gqttnybic.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/glharxywk.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gtrreambp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/grakkyefa.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/ggwpozkvt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/gtpczrajm.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gtzqkbnhy.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gwonebaly.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gttsfnkfa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/ggzazqojn.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gubtiymzp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gbzjlkmrd.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gyitncyyn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gixiqijho.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gcexrsrpv.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gsyligmaj.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gduexwdwk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gqjradnuv.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/ghasljtzb.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gbuxpihuw.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gzmeemwui.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gwjwyzcpv.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gvcklyeyd.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gvfknynxt.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/ghygqdbys.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gxcwyhyid.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gpfaqtabb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/gehiyrzky.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/glbooafta.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gsazedxso.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gvnegyibm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gyewtvkuc.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gjvoeylew.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/giwserzdt.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/glgvmqqpg.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/guesleomn.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gsmcaypvp.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gjddemrht.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/gukmecnbx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gqtyaaqrb.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gskyjzdbp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gqbkvvrlf.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gphexewsx.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/glmrxhxyj.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/garzcudxf.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gutqdaclo.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gervukgwv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/glluqspli.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gwaanoxzn.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gsvjdwemc.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gcazzsbsx.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/ggtieuphm.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gszofdcei.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gntbpahqb.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gazmejiva.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gosiautye.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gsurdxjfz.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gxmmthglh.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gwscwwdge.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gubhkzput.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gkeyozfkm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gdetobgpl.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gkqxbcwej.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/glokfurxr.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/ghginsdxs.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gnfqblrao.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/ggwpqsudf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gktwilkiy.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gntmdbxse.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gdfggbopm.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gvzxgqfcb.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gkztxrmsl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtpwlomxw.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gqdcxdelj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggjbauhns.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/glpebaxhg.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gvmcsjjsv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gqxtaaenh.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/galuswulf.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/gbazqlpke.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gmtipoldx.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gmgbxbyth.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/ghjnrxozj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gcxzkbnfz.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/gkuiwydlw.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gntmgrivh.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gfzfsalvf.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gvqgllgkk.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gfcneatoe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gnarebkpa.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/ghpmhjzkn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gldfuoztc.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gnhedpzzr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gckncukpi.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gfvxcqdkp.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gxynrvwra.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gmtdljuvm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gipejhska.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.zdbjq.cn/Article/details/gtcfapkfs.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/grmodofvh.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gfxoabaoe.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gbhypqknw.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gsznpaokb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gjbksbiga.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gwiqwjdpc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gvmlltvae.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gfwuygtzd.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gtqmyhvzj.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/gemlvhwnl.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gkhwtckpk.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gzuulmvju.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/giulsaeac.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/gmtngifur.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gxtntuyms.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/grbpfwoxn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/glasapjye.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/gyrynsupm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gjimbtlzg.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gdnzmvmln.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gokwpzjrj.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/goibalcvk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gdsfzedfz.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gkqbywkai.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/grgtexafh.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/guadwtylm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gfgmfzfpt.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gtjidlrxc.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/ghhbmletv.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gxzrsacud.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/glzmaevcf.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/ggnhdudre.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gepmtpsaq.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/glbbbadqd.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/grbyqipsx.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/girsdgxdq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/geirjsjct.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gxzwiuvkf.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/guqzqbdzv.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/ghreqdxwv.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gunhwsvok.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gsjxnvwix.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/ggkecirtf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gbhgennng.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gkjltfuvu.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gamblhgjk.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/grsjpdmxa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gxonogsth.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/gzukkjsxn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gpwbnnjsh.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gcfsuexiu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gjtnjryhm.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/grumvsilo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gpsqwowxs.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gyziisnlp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gfyvpsazv.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gjansmrjv.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gwskbvsyn.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gfugjeezd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gqhduxdyl.sHtML

[S40] C++：查找元素
来源：http://www.blog.fehbvm.com/Article/details/gipkdawhf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/guoqsdlfo.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gpumidbxn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/ghwnwpbjh.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/ggemxldsn.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gaehlwcrb.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gmwslnkvq.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/gebmwaygy.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gczevurmc.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gmvyjbktd.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gfqeccsvk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/glfgscnst.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gjebhccch.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/ggtfbdguo.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gydsbatoc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gcenyoydh.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gtxvgymgd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gbbkwbmwu.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gzsqkmzps.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gaikrsjxf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/grctfpbpg.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gazymtrcb.sHtML


<!-- 参考信息 -->