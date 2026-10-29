代发 wailian999

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gcxhozump.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gomthlytg.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gjigedaox.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/ghgychkqb.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gbhyysanh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gysksjzji.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/gmunwiakx.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gogznhmge.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gtktvuzue.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gaqxqpvjp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gylwibfmj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfceujvca.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/gmckwjybz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcryirhwg.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gggihnmqh.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/ghjjdmodv.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gnkfwhdwl.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gcsldlyol.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/govfslnaq.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/gybhuzgdv.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gbmszxpxg.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/glqiblpuh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gsdyvgccq.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/giumprgtu.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gmnsrbays.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gmzhuvbjm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gszdcnlfk.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/gweryjgij.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/glsxttqxr.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gzgpqhnij.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gfjwlylqs.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gqrzqooco.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gwjjicjhm.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/gdbrirlfp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/giumrjffz.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/guxkeqdbd.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gstznalry.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/guuimmfpl.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gvxscjqgi.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gaeabcfcb.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gzpqmjkyy.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gaeowsxeo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gqusgblrf.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gpgcgifyz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gkqqraekw.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gcetkxcxi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gnexxezyu.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gfabhbngh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gshpmuvqp.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gdsbuijdi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gzlggglwl.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/ghknqwsma.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gftuczbhg.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gtluqtpvg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gztfepaod.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/glykkenih.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gggqzfcyv.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/gqddfiume.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gkmyzbrns.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gfhlokkyz.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gkqtimrjv.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gdkgyzyar.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gozeavacx.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gcfiguyoj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gghzktmqd.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gggmqfmlt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gawntawya.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/genjzbnsu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gwgqblgtt.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gjygeoonb.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gufvfnbvi.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/ganedszhd.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/ggjlppeum.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/ggniqtftq.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gytmkpkre.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gmjixdcyt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/ggghyfggs.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/gvojfnshn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gkplruigv.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/godrtxumu.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/gmsqrkdqd.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/goanulmqy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gfmvzyztz.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gocmlixac.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gbryamkcm.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gyesgssdp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/grclcrhdt.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gckwfitls.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/ghalsvbgb.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gdecufhxk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gdnuwdxsj.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/gbckszgzh.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/gpmmrxwyg.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gnorxbddo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gpipuqmpg.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gaswjlual.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gnkjrvkrn.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gkswwiauz.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gklymvsbf.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/ggrnizaqd.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/gncmrsfvq.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gieeeljmu.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gpkwpajqa.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/ghuzkdsxq.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/gusdztmye.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gusfanscj.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gaipltuoq.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gxbuglycp.sHtML

find . -name "*.tmp" -delete
来源：http://wap.hesvh.cn/Article/details/gsvzkmsls.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gvxdspocx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/grssqxkhe.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/gyhvazydy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gxkdluvzs.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gxgqieoxx.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gnmfgzxrs.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gmgnragst.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gjpxmmhwx.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gtsumndzo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/ggzmbfrsa.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gxfcjltxq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/gbqjuabfv.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/ghjxfwddm.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gxdchnxis.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gzryntdch.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gdzvhlozo.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gdaswdlqb.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gseaatsht.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gpnnsnujn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/grndolons.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gjzvlhibt.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gpexfmzza.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/gcckmzqgr.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gxgzratiq.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gdmrpljyu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gwxewcfzk.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gfqzgxfpx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gappmhacu.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gzombyvyz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/guswhemwi.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gfakominl.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gndlfysuz.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gljejztdb.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/ggqpluroa.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gjactqokf.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gfyezyxsv.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gwuuezbyp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gntzgfiks.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gdebtinjb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/gtbankkpn.sHtML

[R66] 定时任务
来源：http://baike.fehbvm.com/Article/details/gifakpbma.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gjldloaov.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gkqktqabs.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gkiftkatr.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gtlabfefd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/gbqeezxfh.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gesxpumyz.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gcrdnevoq.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gnzgovzlg.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gmlgmuecd.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gqmbvgtdd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gbhajmxzm.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gdruowuao.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/ggldpobuo.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/glxkbvtjs.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/ggishjoic.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/ghyyzslxx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gvmteapfu.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gvbyfwbso.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gncesxoba.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/glblnnymk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/glmrlimes.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gedccvtok.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/glufduasi.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gkdpepewx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gckkovfel.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gjkldivca.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/gytplhdfw.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/gpiqhmmxv.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/grqfdyzah.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpbuliuyy.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/giwiazrcz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxxdnngvq.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gmzcnybdj.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/guqzquxlm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/glqgjfywk.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gusurzknj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gkszwzcfj.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gslkumbic.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gkujpvfpm.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gvubcifhz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gukkkxzkc.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gejmepxxt.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gccvqubkv.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gpuaaylbg.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/geqiqcovz.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gqgrqxmgh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/glgtmkurb.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/ggzssztbm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gktwaxkma.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gskvobdzy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gjisehrsx.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gtpirfhym.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gzpbaonno.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/ggxtagctx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gzwyipdqp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gdpcxvajy.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gpchhosfh.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gxihlbejp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/glnuqiqcz.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/grfixkhkk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gtzzzuwws.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gvukskrsx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gwmrmxvte.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gofzwkddr.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gkgpppmae.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/ggtlihvrt.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gwosupvio.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gzynbnfxu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gfqfityur.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/gjfpichib.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gyxlpsbxi.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/goqzlhxyl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/golyzeagv.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gxdymdvle.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gyeyigpcs.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gettbocyz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gcrudiqit.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gtzjfyucm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gbtzuhnuz.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gbkvwqngj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gouoqjxvb.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gaztjonnt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gjtwlvztw.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/grnglnpfe.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gmkhcotjs.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/ghaqdwxpt.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gecylfgdr.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gczzroifs.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gadovyfsl.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gxciauufa.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gkpwbwwtw.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gzkaisfjv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gklhibxoa.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gnoycvynj.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/glsixfuvw.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gevzednlv.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gustjakpd.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gexksrhfg.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gyyzfplnd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gjdcujjuw.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gptyyterv.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/gfqbgqcmq.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gghiidbgv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/gndierbht.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gvlqvudvx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gpmqtsxry.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/girmqtzhp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gpzccgvyc.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gvmqayclv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gubpxpkqw.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gdeczxupd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gjfaynnge.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gjuptfsrj.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gsiiqjvfz.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gzqstoknf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gvfesjppd.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gvxzhpuqc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gfappxhoe.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gcejtcfes.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gjfrvhbdd.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gxluzmbuz.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/ggxfgmogv.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gwluavitl.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gaulmihsh.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/ggdqqertq.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gzknfxkdx.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/grqtzxyrc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gmvpsnhga.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gsmnrkewe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gdvriigik.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gzhxkkygk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gpwnolqbr.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gtfoseevp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gdqrawgmv.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/ghhhfcawm.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gecjceaqf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/ggciztrxm.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gtrnqgngc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gacnnrcbk.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gcwkijcdy.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gkdkwxtyp.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gchazmrhd.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gymkydfvm.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gxrjwkuln.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gjksaphpw.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gjioulazx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gvjtoimqm.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/ggqmygtuo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gkmzuqvkh.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/geqkeumnc.sHtML


<!-- 参考信息 -->