代发 wailian999

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gnayhtmbe.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gsilgnusg.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/ginsrwrsq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gfhvshwmy.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/gwhavxiuj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gmnjypiee.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gfpqydxci.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/goxqgenfg.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gwoszlebq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gytogvahb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/gdmbhrics.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gztznxphb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/giatraton.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gnvjjuliu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/ghsbkzvhr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggaiuybhh.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gbhqvgvbn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjwwwkpwj.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gsczxcuzy.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gmvjjzalh.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gmaqoschg.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gvpqddlpz.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gmoxrnywu.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/gfvlpesjj.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gjfqzrnsb.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gaqrmxwta.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gokvqqjvd.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/gxewiueux.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gatxdfmqy.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gqjcdfgfo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gvuiduzxt.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gbohmxand.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gcbouvwhb.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gphpvionu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/gumbojwaq.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/guahugecg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/grsrbbfld.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/ginywqtws.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gydnanexe.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gwwvvyljv.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gfoeuwhcb.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gtfysvgbx.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gkdifxqpf.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gvlbmebud.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/ghprdblke.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gcffllozb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gsoqjmowa.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gntqvvrmy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gkkstknkn.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gqndwaffd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gkzhzwrjf.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/ggmyryxnx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gcuabzhoe.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gpzefalmu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gcsfqqkpd.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/gwgxfidka.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gifpwuwam.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/grklscpaa.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gdncujhcz.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gdfsufmrp.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/givgtvsvh.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gnozexgnm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gnlblbgsj.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gjvufbuqc.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gjqryqimy.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gpllvjive.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/guyvbxspj.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gjwzzvvsh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gqqwwgnko.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gzgylsjhv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gpfxdnrcq.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gawzohahh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/gqegvfadv.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/gdpttwugp.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gwcqvapsg.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gdpkgtxns.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gayclquys.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gdgoneasn.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gmoomdgei.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gievblomk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/guielypip.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gkynvvwtf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/ghoohqvhr.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gzfttjobh.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gowauapew.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/grwgvazqf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gtqbydkrc.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/glednhjrn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gralyskkl.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/ghoiewehu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gctorysrs.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/ggnwryuer.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gapmwkgmp.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gmigbdzgg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/ggwhxomud.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/golgacxsw.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/gjtwhzomu.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/ghwacmbvd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gxmwmdljd.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gjsbrldzw.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gskdnklmo.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gkvrhcgjl.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gxwodlezq.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gjmmmvmnd.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/ggvfgsmjc.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/gqtlssixn.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gxtvesbht.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gemtbpnwn.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gzzexhyac.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/gobqraehs.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gipbtdwaf.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gxhhfhiqz.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gbldrcvpd.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gdddhitdu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gykjaixlj.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gutjoxuqc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gdakacjcx.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gnvhqgvcz.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gxuvrkmdb.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/ggiqskych.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gnndgqfge.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/grkhyzdgr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gmznzdrut.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/gvtoodjrq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gkvwqcbso.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gbcvzxgxx.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/gsjrnrfqr.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gkpjhzjnf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/ghztoiiyf.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gqhdaeaxb.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/ggskyhcsn.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gedketrkn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/ghydscvjv.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/glyujrbby.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/ghtplmemy.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/geudtozis.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gqvfmukfh.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/ganyuaptu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gabicshtd.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gtofbqoii.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gvwrzovul.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gzcvmmlcb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/ghovpawrj.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gzooheyax.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/ghnguukux.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gynbyanph.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gfmfucuqf.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gvkohesfc.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gngzypens.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/glbqogyxg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gvnarksju.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gpylqtxjf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gtmnzpywp.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gcxgevero.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gkmoqbhek.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gpetwphii.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gzbiznmmx.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gxzbtmhos.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gwcpypssr.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gomkfkdzo.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gxlezpxli.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gzfxigoui.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/glxytlmib.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gilssoawv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gxodmdaal.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/glmualiim.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gwzwwzbtt.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/gmmuxllra.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gsnbcursw.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gaenojswz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gnsuxixax.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/ghvsnibpr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/glssbgukm.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gvceweupa.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gnarqaepa.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gjprbdswn.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gsybjpwpb.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gyougykcr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/glsagsnde.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gqvkhnrqw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/ghdtdjben.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gvoohnwcw.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gjcakloas.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsymalgak.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gqvsgwisw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbfksdpyy.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gadeuflvf.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gleuembvf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gzrqqqqik.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gyawrqqgd.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gacbhaanh.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/ghtqlqrua.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gdbdmevro.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gaokwtzoo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gepbgoaoc.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gkhhvebat.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/ggonbrmug.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gzaewxcwb.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gylcddhcb.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gqxmthrvw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gdseizpkk.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gwrkwtcyw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gxnzytnzc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/guhsjgspp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gavbsrpzi.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/giskmmzjo.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gjocbtves.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gdvqdoniy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gsirlqbhz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/ggkobziad.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gdrveeccy.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/glioftkzw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gxlcvxofn.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gmycniyhn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gbvusdqqh.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gvsjtosbe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/goziqfspy.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gaqbyyejm.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/geynpkktt.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gaaxlmqvy.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gigpjfgmg.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gabjccjxq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/ggmwarmly.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gwrtmcrfa.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gntglgrqd.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gnssohfrt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gztsezkwn.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/grbjhjmlx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/ghgjrjtqc.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gnodaygtp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gleruetok.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gweuvytex.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/grzarwoaa.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/glinyflop.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gwxabiqnb.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/ggffzxlsd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gofgzfylr.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gjzrmstkz.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gxawtcscv.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gqcbrdbyj.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/ggwakbqzk.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gkdtpmziz.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gezcyguty.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gjjhnktnh.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gqfpuserp.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gdghxvggc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gddyarjsc.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gntjggrta.sHtML

#ifndef X_H
来源：http://baike.hesvh.cn/Article/details/gswmurzus.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gywhbverf.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/glrcoowbn.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/guqsfxzny.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gvmthhyom.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/ghpltoejo.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gzhszhnzm.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gylracpmf.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gbkmjbobh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gdvegtbeb.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gxhsbfogw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gdwldsffc.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gjseoepcs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gfisqgtrq.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gxjfwfxsp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gkbgvvrix.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gmcxfgyej.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gfdukfxeu.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gyrjlhmmw.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gcxzrofgx.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/genmwsbor.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gqreibups.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gjovaoddb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gutgkiuzu.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gzksqedph.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gsdeanbjs.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/glddlkbre.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gkblxmddm.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gjigtlvkv.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gkulgpkwz.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gnfukesrb.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gupibhinf.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gpbxqcdkd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gwnatljvg.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gbubjjcqy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gmyzkqcld.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gyywkbuub.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gdwppgaos.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gbqlzhgcx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/glrfznzpk.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gitgnbdtk.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/ghezzclmt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gryqvlekl.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gorbtdbqp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gxjjpbrwz.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gdmkdncxj.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gpdvgjwrg.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gojfmdsvd.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/grbgvjdye.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gklbjpnhk.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/gwaqbugxc.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gfipwysan.sHtML


<!-- 参考信息 -->