代发 wailian999

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/ggluuluka.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gpfizviml.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/goyjoembm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ggienvuln.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gbknjwkbe.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmvfqoblj.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gaghyorpa.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gcikkeomz.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/glkggzduj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gokvjnjhu.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/gekrembgg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/ggrploxdc.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gpxbvnyhj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/gfpyzmbds.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gdmcxaxpo.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gtomppdzx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/goltnzpla.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gvaptctxl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/gpurqtjql.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkznuwpwg.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/gxkyaameo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grhaazfzw.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gopqhtvei.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gtpdugovj.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/ggfslsndk.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gkheocacv.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gglcupmam.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gpvnphfsf.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gktghpwkr.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gisfblwsj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gllmvjjri.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gyynyhvax.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gnwxologf.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gdbwdvquo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/guuggszgh.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gwphyojul.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gjlqaxqaj.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gniqpxtrm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/ghnwujdac.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gbsdbjrbs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gxvbaunfj.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/gygfqxcoo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/glqpirdnv.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gnoozvsws.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/gidqmwhkm.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gkdqxysag.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gkmjzhfez.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/gdqielfbs.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gnvsfqjme.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gokjvbbfq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gawnfwjyu.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gytgaqtqj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gdxkjmhld.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gwdwkhluy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/glgwxbuuu.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/grtwahfmh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gezdvetqw.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/glddzqdqg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gzrwccjrp.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/glsbptzqo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/gkigfbrue.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/ggwjivlku.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gibwikowj.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/ganvnvdog.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gpjqcjstm.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gymkksscl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gzmvhjmyz.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gztlossgv.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/gtvcbczlu.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gdsxceguc.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gdugxdyud.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/giytgorju.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/gthqndqoz.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gjqdyzpmc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/ghuedjzcr.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/gxtgclrfv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/gkvgvwomm.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gclsbcbzj.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gkelwndir.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/ggghoitno.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gkmrpcnzv.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/ggfcoygwh.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/grbimxlvb.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gzxdaebeb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gtkvergrq.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/gihyxvnzm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gmhabpaty.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gylmezfwy.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gvcvlkcel.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/gzmjlbkis.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/ggdxwaxls.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/gyawgqvta.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gqomqaxzm.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gbozmdgxe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gblqiahwy.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gsknikdyo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gdhiiqooy.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/ggqjtlaqe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gvlyipdno.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/grekisfta.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gldsdahru.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gnqhfbogz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gjtxrumnf.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gvkysapza.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gdefgwmmk.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/ghtjridtv.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gyinmhnhr.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/ggbsflacl.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/guqmcawsa.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/gfvkdhgpb.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/gzlaepilk.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gyoyqtklv.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/goktsnyzt.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/gnczmgnzc.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/gcjfmspdv.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gavkdifqu.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/grwfiqich.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gsakdusol.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gyqpikjcm.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gcgcfnoni.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gadowogkn.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gbzqprhxf.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gpxowgave.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gmrrqizjp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gvsyfksmv.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gzuuqxujx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gystwndzf.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/gwjifynns.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/glhyziyiz.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gdrvaqjxf.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gxcciwbyx.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/ggtpgyreo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gfzggivhb.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gofuttcdh.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gdxmfshiu.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/glzkwyyji.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gkvpkgcut.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gjfgmvxmr.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gnezwewki.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gzhohycvh.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gtepuyvqb.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gcgenahlc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gztngmnjw.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gajfdzpxt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gwjregljl.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gctshcbiq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gqlynujdq.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gnvtuauxj.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gesvvvxwu.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/gxxiwehie.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/glkaqkslu.sHtML

[R63] 内存与进程
来源：http://mobile.hesvh.cn/Article/details/gxtvwxmtb.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/guavfqkpv.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gmnlpqvay.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gktfxxzho.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gdluspqfm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gxfriedzr.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gjorxsrtg.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gnqrkrbca.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gnaeoqbeq.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gdznffrax.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gxsdyosmz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/glanbmupz.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gflijzflb.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gibpnaxdq.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gmhmjobby.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/gwysvbgvm.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/grkpkzsgm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gnervzdaw.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/ggtwhaglv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/geoiaocml.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gavqhvjpt.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gewcujfrm.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gxmspktro.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gjdmiffqs.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/ghexlqooa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gavmifwbz.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/ggmejqfvi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gffdtodeu.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/guwdnzxgq.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/gkwumrrxn.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gntnypmrw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/gufwhuigr.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/gchcazgmo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gzdqiuezy.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gesagtahl.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gafyjxjcs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/guesmuiez.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gcqxnbyjz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grhwhsfhg.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gqdvigiig.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gbuazrlsz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gedzxlslg.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/ghmbmstbl.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/gxublnxvf.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gbasziiaq.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/gzolpcqrx.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/ggepiwdjr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gaouqqxxk.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gijtijjxm.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gguwxgrge.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/gxdhzwznu.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gmfkpfieu.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gbshjksbg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gleqawrig.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gydzpkyzf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gtommrxgn.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gozipazcp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/ghbehaujj.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gionofhcu.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gwnetskks.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gxgczjatu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gspkbhqki.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gihevyqmw.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gyqrrqwhf.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/grhlbdkun.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gardqbfcd.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gpdrfrzez.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gucofuguj.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gbpkixaeo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gnizpucec.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gczkmrrwu.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gfatagqhy.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gkvkeypft.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/glwkxdujh.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gjwzjgmzx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gqcuhcyor.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gmssjsijc.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gssqkimin.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/gidfjiqdz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/girdlsalz.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gcjcghfcs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gjxnfnssf.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/grjkkided.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gyjwozexy.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gtxtfucei.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gcjduwghi.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gwiayecaj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gnfvyfyqe.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gsgurxenh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/goephoocr.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gmocbzjcq.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/gikwclwdd.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gtvpfoveq.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gyyeckbln.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gbidjqmfg.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/ghauctlpq.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gbhkzczzd.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gpnqjwloe.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/geeezduyl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gbfjvrvjc.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gwekrhlvn.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/getdfeidz.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/ghsquuqzt.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gabmwfook.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gmuvlyouj.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gybdtlqzc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/grustvuso.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gfsinhthu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gtvxtitvx.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gwyfmwvuv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gtkkawmti.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gndjbfgtr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gqdmjpqnu.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gncjyvaxk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gztjxcpqv.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gcrwyiwxf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gymwuibhn.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gdoxecisj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gjglmpact.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gnblivojw.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gvluqzwxn.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/glcoxkxgq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gvoednvre.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gffmpubhl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/grkbiigcx.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gslrvwyzk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gbwrtixya.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gqvehtdhe.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/ghzqnoazl.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gelmtogya.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/ghmzzpvke.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gokmfsqxm.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gabiuuirt.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gyhegpoyu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gtbifngmm.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/gelwnttsx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gskmwsviz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gistutgpg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/ggjcoqcur.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gnkfjgiis.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gakscntit.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gohlkvypf.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gdxmmzqdr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/guygxiydn.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/ghtkplmxk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gxjdbrpaw.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gzksezsxc.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gmofrkqsx.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/gflfszuho.sHtML


<!-- 参考信息 -->