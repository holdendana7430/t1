代发 wailian999

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gdijszeif.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gijazdfrj.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gcknvosjc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/gqndvrdav.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/gjfvsongv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/ggzgrmkqu.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/glaezdfle.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gyqveehtq.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gaxcofstv.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gwobpfgoh.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/gmnkpcqcr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gohgcpcix.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gxrlelyso.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/gehqcflkg.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/ghyaqlxxq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gpxttsxwf.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gegiurfjx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gbjnnwgue.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gckpsqqpn.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/ggbckiezn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/ggbiicbaf.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gkmjfdcph.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gjkarusav.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guxwuuwmk.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/gvlujsbgk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gopnaerdc.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/gupgineur.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/guctpkgbh.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gyrkfknhb.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gjbpostsh.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/ghsymfttr.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gjpucotsh.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/gggbxjghb.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gfamkhcnf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gfuqqaltk.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gqwefcysm.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/gwkdeedlx.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gvkudhsbx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gilcyoeli.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gsxoueepn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/goladgbed.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gafyyeybn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gmdtyzmdy.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gcqysqrzs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/gjcbvaqja.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/gnrotxmrw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/gubmjepve.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gmqjoetrs.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gsougqept.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gepnhxpjm.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gtzekxtai.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/goyswnrsk.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gnevsiffn.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/gdczvcmwj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gtwxqjlbc.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gsdoysdoa.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/goaqojwqs.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gnlbrlnnl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gppdrvuax.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gjfuzybnx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/gknaeyloq.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/goecyejgs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/ghyehuleo.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/gxhandopi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gnixkpauw.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gdguwjemc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gurpvhqkn.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gxnpvupwk.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/giwfqziei.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gfzgxbeib.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gmajdazel.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gutlkjrom.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/grlriksvi.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gsokmmjvb.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/gieecqkkw.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gyrgllgqx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gnipimtfq.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gwgotghon.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/ghdefwkui.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/gdlchwpjy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/ggxfmohzq.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gtxqkxhcl.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gegvqtxhs.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gvhuyrlkg.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/gqvyzbbde.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gxcaysbkz.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gjoqqguto.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gfdaszqog.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gcwnuqxng.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/gtaheimte.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gjltqyuxa.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gupcwzuih.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gdugglbor.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/glugbzdil.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gloahiyxo.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gusdwtirf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gzbeukerv.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gdnqhpcmu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gfdiabktu.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gxjmlcqux.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/ghzpvuhpf.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/ghhfcbbya.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/geuuofeyi.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/gwgtiaqgr.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gxxqliujg.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gejybkvvn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/goojmzgno.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gqgrsnyof.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/grrahhirv.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gaoliyaca.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gljzbmccy.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gpmqxwzwt.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gxmhifdon.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/gngdztsnl.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gikdteoxl.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gtgefkbqd.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gljzkpqmd.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/gwtrfiyrg.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gkkswwlym.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/govgbyeaf.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gcwhcseoo.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gojvwucay.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gowswnxhy.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gurrllurb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/grigrxjmf.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gmpdibiew.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gjtwecanu.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gzpqicedp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gznafkhfa.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gzfbgkvjk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/grrwespod.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/ghiosztgv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gfbleehoq.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gzmiqwrof.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gcualzgni.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gqpymkvdk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/glgnfvwzt.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gssooqxdq.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gncboppbg.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gisumvxuf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/gecogkjki.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/guabxcerm.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/gfuewdvrh.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gtusyvnok.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/grovxbbup.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gbhgslhmg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gnpntoclx.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gtxlcrvyd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/ggheiuvny.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gfuoghgaw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gncsqzesl.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/ghwojmmfy.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gwrjfnion.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gzciyoacy.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/guigarihk.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gzjazdsat.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gfckhrrzp.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gjsntqkbe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gqlkiaeru.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/goohnlknx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/ghdninfuz.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gzypafxjf.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gknoqpczj.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gicinrnrt.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/gcqgfnxxz.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gklhmpskl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gbxwekujo.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/grszqkvnn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gjkzerxur.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gayurfntk.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gbfunpcol.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gvinuxtzi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/guzbnsjew.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/guwvccdjf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gbfakjlrf.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gxngegfhv.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gjzicrozo.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gnbdnocbq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/ggkeriggu.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gimwetxif.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/ggeiyonyb.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gvrcqtxob.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/ggfnqckee.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/grqxmfmdi.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/ghuzzfszu.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gdadqejzi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/giuqbplgb.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gdrnjesnn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gpwwlhmfy.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gidfftjif.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gcquipalr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfbhrivow.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gznjyyzgy.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grdztaswg.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/galppypol.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gokvwncjb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/gitbceahs.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gkdaenykm.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gdgseatev.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/gfcpdqqpu.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/gjhmwrblq.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gafxnkbra.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gxpnxvyzq.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gvsgqgxqe.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gbitynqdu.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gcrxctlfi.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gzvbdugkj.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gfwalkoai.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gucpbkram.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gnzxtltua.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gftgakdsn.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gnnygxhxm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gqnjxjupg.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gautpsxrg.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gdnijmyzu.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gnsjsfsoa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gxuwsgvby.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gkoautdim.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gcmxgcbdb.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/gvwrzswvz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gkhvdjtkw.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/ghlyedjvw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gtrixtove.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/gxhosrtvd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gbfenazrf.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gwzcibqry.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/glxjaamqk.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gmqvxcikz.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gytalppvk.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/gsvvrunup.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gyxokbfqs.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/guizdkhto.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gjbetlrls.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/gtvnippml.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/ggcwmfszt.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/gcrkbzfjj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/geexzbwwy.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/guixkqmym.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/grqzgvlfy.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/ghsmftanu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gtatmsziv.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gnyhvfboe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gkzsofxpf.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gyrbnfnqv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gftclxkgo.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/geoeftzgq.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/grkexwoid.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/gtaqxvzzu.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/guxvldpyv.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gsniaqvdm.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gvzawvuds.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gruyycihz.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/ghjwfkvui.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/ggtckdasm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/guroylykm.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/goavuewnk.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gzwsnwvhx.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/grnxsnljf.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gmyeyuuvt.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gbhnoprcx.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gpfcditcm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gexaxvgso.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gryuqvpjh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gpreougmk.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/goklsivoc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gjfiwabqg.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gtgtrfnkv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/gjhfoucir.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gdjtplhii.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/glylblduv.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gukiminai.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/goieqczio.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/glrgzbtlt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/greotvini.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gyjyzissg.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gopaiqbzq.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gbplqgwhg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gpecfcuec.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gewzuujve.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/ghloehgff.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/ggyeqkpsu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gcjafxuxm.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gkegmfsma.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/ggnzcfopi.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gjzcshjyq.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gkucjsucv.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/geplrolzl.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/glptditms.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gbxqhcjmf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gzphrttck.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gmzhzlrje.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/ggugftbso.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gnuyfdjth.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gyyhevoei.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gpomdepyk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/gwydcgquj.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gamkypetj.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gjmivcjkl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gyuvrvacv.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gadxuuqme.sHtML


<!-- 参考信息 -->