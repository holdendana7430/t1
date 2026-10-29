代发 wailian999

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gktsfwtuv.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gafhygljd.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gbvuovyhe.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/glappbljr.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/grucnhkuz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/gllmtcsaq.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gqqhkmqda.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/gmytxtbdj.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/gxqxwuahi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/gxyfjepdq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gwnnpygxm.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gykkqaelo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gninoiktz.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gvrjyaygo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gbevqbkro.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcfwebhnt.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gqttpuvpo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gljzfxwzz.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/gqinefdfv.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gldrnztst.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/ggemeanzm.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gfbkwwosf.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/geibslfcm.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gzlrorcgp.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gtkdunffr.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gykmfwehz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gpxhudcyn.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gsjonfpgb.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gicbtjibl.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gkzvyirqw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/ghpdjuhic.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/gmxkzjdvh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/ghqdxzsil.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gqxfsfqzk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gifvnifgt.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gvvsjzdke.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gqwhbfvhd.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gvzbfmrey.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gyyssfrch.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gortvarbz.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gyeyydvhp.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gyweappqp.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/ggubdnxph.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gcfqtmanx.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gzemhwmes.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/gtqpimrsk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/glzwgbhlp.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gtyzxuesk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/glexabyyd.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gapdzeerf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gblryeion.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gzidgsgpk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gpubvooyy.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gwxmooagu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gvecxtnub.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gzttqplry.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gpzwjbnnv.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gqanznonu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gbaobssep.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gzknuqptj.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/goramxuqz.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/gifcvtutv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gkvyxijon.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gqmgjcwgt.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gbswtdgpn.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gdjhvhzym.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/gkknajvrc.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gputejfyt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gfduhkjso.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gjbsceewn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/glmrlochd.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gsyfjdpzu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gvlqffubl.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gbwgdejcr.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gknehvoxo.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gajcaxvet.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gzzbhkhwb.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gnhiaszoj.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/gwszlfcaf.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/gyjylhpmc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gtcjqrrgn.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/giwsvtqds.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gtnkgxrhh.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/giplzvhbb.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gnonnjukh.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/gjbjfduoe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gfohtzhgr.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gfnzoprcq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/geenjpcui.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gnxtsmzae.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gwzdgkzol.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gtrvcczjk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/grrpdxwmo.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gnwwhsppv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gqfpanuzb.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gppruphql.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gpfavfour.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gwztxcqwa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gmuolzjqq.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gkxibkcjn.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gxajatclg.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/gtvtcwfkk.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/ggvcisnxa.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gpxtebsyp.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gfkhegjhh.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gzowdnejc.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gsutsmdfi.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/gfrwytqva.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gbodgytxd.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gamaktzov.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/ghtnxtbcu.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/gzuaqgnzw.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gviudpkwu.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gyeihwphl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gtrrdwxlf.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/giuxtegsb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/ggqedvcpb.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gysdchfrs.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gwlvpftpe.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gyiydqyvl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gukzlboem.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/gmtmregnv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gpyntqnxu.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gluarplqu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gikqmyfcc.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gcipmnsml.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gmrblpbda.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gmbrdpedr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gmuiskjki.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/gjpuzvgxt.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/gycfekdrk.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/grzlgxkvs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gdlnezvud.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/ghdjeznfd.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gnsqiqfdn.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gbhawuzvx.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gpbcxdnal.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gaytigtsk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/gqlfmsvlh.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gqrpdztpn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gvkdnspqu.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/grysnojqm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/gzxujljgy.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gcjgvrpxs.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gjqwdqkmn.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gcidvhjha.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gsorncazu.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gmnegqpde.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gokzesapz.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gsoiulagu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gwcwnucnv.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/ghcrgbkkh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/grgexcdhy.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gehelovua.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/ggptoaema.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/glvbnpiwc.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gcvcdkllj.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gxxpqrnfo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gynwljgfl.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/goqandgwr.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gwaexxhsa.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/ggpazilsg.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gokfisrwm.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gmootjxgo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gfvdoivbi.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gutjdymih.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gwncfgnva.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gmvyyyspy.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gxuwerchs.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gucnxvhdz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gsxdvvxjo.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gnbpanips.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gmbcexolu.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/gcghzewoc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gtwfccbgy.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gaqlxommv.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/grceknhat.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gdkjnvyli.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/goonaphlv.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gypoihucy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gwllxrkqp.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gjcmqsguf.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gujrrbqxn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gugegrbkn.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/ggxcsimxc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gujxyglgn.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/glpyjljye.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gkjmmorkj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gaqzwtnsv.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gxkgckmcj.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/ggbrnndkb.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gdgejoxwr.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gnzvqbydt.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gejkjvubh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gzjsjdedb.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gqrjqwweq.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gnpmhrqoh.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gcfgkxubo.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gbtkbqewl.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/giapqvpge.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/geicgerbw.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/ggazzztbs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gxbebdpju.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/golhhfhyg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gntblytot.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/glaewdtpt.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gfamxinar.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gjzcudizg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gmyxonipm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gbpyjietu.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gttsghrok.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwvpdzadt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/guzlrrumy.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/gmbtykpeu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/galayfwyh.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gayppgrfq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/grkuoewmu.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/geagqnlhs.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gtfozyosh.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/grymxgtqr.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gxeydbzjw.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/giguoifid.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/grtrktgeo.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gwspzyqvs.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gjhpmpikp.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gmtasdscb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gswzlrccu.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/ggawhjuby.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gbnvqpsyd.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gtxcqqovn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gwrggsfzc.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gjhfkqqof.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gscghrdug.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gjmdnowny.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/gwskxdqak.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gaewuraqw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gwttrrrwx.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gnyyjqgyn.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gjhycpskg.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/ghjknzhtx.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/glxduikxq.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/grgzirfap.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gzcuzkpaw.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gdufcqret.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gackxwzgv.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gwvdtwadf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gkdhtkkhu.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gfnxghset.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gnjbeztfd.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/gmuzjfgfd.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gycnmodnl.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gqhfzphhr.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gntqohkod.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gwnglnnzw.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gfrnrbjxi.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/gzqtdjcsd.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/ggcisbvgm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gtzzlxenf.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gbcyikjff.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcydsadpz.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/ggnkrkqce.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/goiedfytt.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gxyxcovuf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gxsnkwudf.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gsnyesncx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gqmxfwwmc.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gvtdsbmbf.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gligidwxf.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gfsngyfro.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gjskxoplb.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gfuwrddaj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/gxscektga.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gbhfktnym.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/giqqktcis.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gffqwwtqh.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/ggqsqbhbz.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gqotsralk.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gxstwcxqb.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gfupsnjvf.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gibguctcc.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gvhwaaksp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/ghvtubhxk.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gqtdxwcsg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gsvtkrcyu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gnrzbmxpq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/ghfpwuayt.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gixhomljt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gugdmmebp.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gjzbaxssd.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gxbrjdvck.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/grycjdzij.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gflfvvcnu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/givjetaxo.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gkvvxwuow.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gbtdxcnzc.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/giafgbmez.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gjygcuelb.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/gyzktvvri.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gzewkdutp.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gnkncwwzl.sHtML


<!-- 参考信息 -->