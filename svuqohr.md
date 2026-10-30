代发 wailian999

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/ggdgyjxig.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gwrstkicd.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxedhhvl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyziqgjxw.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgivkurz.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gublioqmq.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggexlckue.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gabptxreg.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwyumidn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/glpqnnduv.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gdtljyplf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmyfrwwb.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvckoovk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gtwomcwxg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/ghxghouyr.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gcolzupbd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/ghmiovnfc.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gippjseyc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/ghkcfppnd.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvksblkk.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdppfeap.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgexhxlf.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxxghavh.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwyyqvuo.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsulsjhe.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gnwyviegd.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/glnwmqwbm.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/ghzoufehm.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/ghpmwxskc.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gedsbbhcw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gdyazgodu.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gsqmpmixp.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnejrzihv.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gbbxajlnb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuntwruv.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvuofhchd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gnobtuwuq.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/ghheploql.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtlhpvov.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnaxyffpo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gsftscqyi.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerwntvjf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gyvrmbwlj.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/glmaoeueu.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gltkpcoaf.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/guorhedvv.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpchwksvf.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gmuoadmop.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/glfhwuqan.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcxpknwj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/guzizovkb.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnvgxgtp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gqstbudsu.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gppqhcchd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gghrswmal.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmpfjbrgm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gzddefzde.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gorpndbsq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/grthmufoc.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/getpitwas.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaokugvwe.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvysbczi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gxilyvkwn.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfsjnqva.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpqptgyk.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginokfdjn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/grpfhclis.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gtuxnrblj.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gjbgticnd.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkpdjbcn.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gezoeuljf.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxdhnxxv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gipcwqscs.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnctingf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/goptmatgd.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtbghohr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gcwpqmuqv.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gbilmvgbe.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gzspvbqfb.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gwhepjoey.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gtozchsul.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgyqubbl.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/grxltdzju.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gjafafnxx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/glhhmfzfw.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvzpfgph.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gesbsouyl.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gothyrjvr.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gurvisryy.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/ginifrrtn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwfgwpvb.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjkkfbif.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/glhuausjn.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gxuqcjhod.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gfgfjfnji.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/grhwbvksl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gjkyhlodx.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gbaxxwkyb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gnlpqvtbi.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxhqrxey.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqlpgroe.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gmchwbujm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbawkcej.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gkudxrfqw.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcebpchrh.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyzfjxux.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggofzutcd.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlsxwfzj.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gvvuenrrc.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gegytszju.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadzlbfsz.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvmypqkk.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gejqflila.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gxcazfofm.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gacvsdvvk.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gbtskotwl.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gsfieyomk.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gtckxscuk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gacqfewar.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gbmrzdkas.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpbujvvr.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gcaqdqzeu.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/glrkswaqd.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhepexwg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/goougkguk.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giciogpef.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnxiudof.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqckvjoa.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gacbnbtbx.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxlfispd.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjugspmhq.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gidrlomtj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxuegznt.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gagggdysg.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gaehzmngh.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrlnkujs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gojcwofvl.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgikhwdl.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/givdyznoa.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gycfbrpau.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gtjabejmh.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvmxdynmf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvjjodvw.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyjqukgv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gknphuzdq.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gueyazzbi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdmhlobt.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gzeihuimz.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gtavztbwj.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gfiqnkwma.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gvdaebrsi.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gqhgdgdqv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttfacfxt.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gzkxgwynw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtrhkbnd.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gtopqjree.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqswxjgbw.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqdrkdju.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gihtekuvo.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqiecark.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gsthvelwn.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/ghuwohpom.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gymwscrds.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzpgfnqg.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gcjykynqq.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbizlfst.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/ggegsrfum.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrvvpwll.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzyspifk.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkgagobt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gokcpxkmt.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnbsqvop.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gwjdovvcn.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcvwbslu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvnortyk.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gtxurbdzm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrfxtipi.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbsigpkr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/grssamnhf.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjlcoqyw.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gmqdgcmtz.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwsstptk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gcfefprqn.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfjnyyfk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpwlnlvs.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gutncslia.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvslhklb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqphlekc.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpyugjvv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gihisajfe.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gknsgbiuf.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gfjbruxaa.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gendmytqw.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gtbjgkktn.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudbsmapx.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfrputqg.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/ggoxwcpbb.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqahsgtq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/grrgyugpq.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqckuait.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbhqkpqm.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gycgfdwvi.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gopncdykg.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gfaphfafk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gezlbcgyb.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gifqivusp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gzulcquyw.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzedewsq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/goqxntjzj.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/guwnujmke.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gwzxlllyz.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvbmaqvxs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gfknsnrpf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/glxsgppoz.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gspdbjqts.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyatsywc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlkcyeje.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/geaxlaqqg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gvhryqnwe.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafbguiir.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gnvfkctay.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/geusbclkt.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/glqpcjhcr.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gytvojecd.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/ggrbrjwjl.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gqmnpyjvo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpcchefc.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpflldje.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuwlpaou.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gptwpxoko.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gskkymdbr.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnhgeihc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyefilned.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gtlnuhlpj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gpfmgtmir.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gzxpkrysr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gugnmpmwd.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gurjrgipa.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbnvtlec.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtitesrw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gqvgqtwae.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gedvckxyh.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gicgffxsy.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gowgubeac.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gftisbdwg.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gigfezmbw.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkynsavoe.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gmduyuqqn.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbejdspph.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhokcfsx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gfixnexct.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gbncbvuqp.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gjseyuhjp.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gxaknsdip.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gimlewfwa.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhcrskbd.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/guvefxpid.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgqmhgtf.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gzezgfobf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golraeodz.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/guzmsmsqx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gztplnxxn.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgjfceid.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsjeobxc.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfwacwyi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkwwilss.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gdvdkehgc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavsukkqj.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofkcmiah.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzcrcwyk.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgmgvevq.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjeezhjr.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gdphmvylc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gutlwkrzj.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexkgnjxm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gookjuuiy.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwhxamfw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gkkfexsrm.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjkmccgk.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gahbbwmzx.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxndqxaa.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gewqfyhxj.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/geemtijpc.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gprhdwrri.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gnnnjexpc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbahpxvk.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gjvqgtllu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerunyszm.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/guepwnfpp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtramnoqt.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkwaiwcn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gviyjvdqr.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gtryxmvas.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/girvldekr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdfclqvd.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyroveepx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/graoshrsd.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqsvslqv.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gfibqhxhh.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gtabgoxbj.sHtML


<!-- 参考信息 -->