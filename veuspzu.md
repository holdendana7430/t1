代发 wailian999

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gvgedecpj.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gwyzkhxkr.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gtdbtesbh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gsosgrwnm.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/glulkmjcn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gbijsmcqh.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gbskubsvr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gmfcqatvs.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gfymbjfgg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/gosrzfibj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ghobaumav.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gcmyorncb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/gbkstgkxa.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gmonbkibp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gezueqcld.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gseyybhce.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/ggsjdgcet.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcapmqviz.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gefrqzquw.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gtbnsvlkw.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gcvaoovib.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/gndcuybmk.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/gkdbmrzps.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/gmbjrvdom.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gntssnsoj.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gylbapqih.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gskcdxbdn.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/gmtrrlekh.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gamtnuesk.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gcgbuuixp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gfzfxbrgn.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gccvnvvxj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gbcnzclxf.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gfipdxabv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gutqrlcfe.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gpsugefsv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/goefabntv.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gsnjxaodn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/goaobrljr.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gicighfgw.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gefzevrxo.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gxvpisrxz.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gulrlcare.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gamdrxofl.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gplaonnpr.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/gbcwebejm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/ggibwrsch.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/giqmizfhy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gsxommgdg.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gzuobfuut.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/grprxolvf.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gmvoquqle.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gsopqbsbk.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gtgkvctqy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gewowrelh.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/gdhzidlwe.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gtpkmyjoa.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gxwvjbsfs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/goaiqiakv.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gnhhyljyy.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/ginxhngqi.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/geqjjdjgc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gitbrikrx.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gkbxctieh.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gckoyffmd.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/goiuyncxy.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/glfcnknmn.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gxgorwjah.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gxthcnyka.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gbibyaxtv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/giwontdpt.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/gxwunebai.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/ghjaycrvq.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/ggwiddzlk.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gywsnntjf.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gsgpnsehi.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/gaakluamm.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/giwknlodv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gemuyytdi.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gmmfzcwtp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/goumnlqqz.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gqdzsrcgz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/grebyzkye.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gjamacdrw.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/gokyywiei.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/gdfpbxgiq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gwucsdtqx.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/giroajumg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/glxzoleso.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gvylamonq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gnxnguyxk.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/gyzxoxyxe.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gcjtnexkv.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/ggvuwfnrh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/glfhxubcb.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/ggtjtnson.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gqiwrcqyu.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gcuifdtah.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gxcfubdoo.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gdyjlkwsr.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gyirnnbtt.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gidirlfai.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/gappcerqq.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gvfxgaqap.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gceiulwyr.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/grnxljayq.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/gofvyrvgf.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gingrcpcy.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gakudiwcz.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gnshslmle.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gkixamixp.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/giwngnakp.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gwbkhqixt.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gdwpzzmfn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/geirqjvbl.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gahclgytr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/ghcwzcgdv.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gnmpklotb.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gwwvxpnak.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gsfbxolee.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gbuexfcdo.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gvknpfmct.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gxafhdovv.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gdyowohbh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gsnypnjxs.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gjhrddqzt.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gprshmkxa.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gadumwbah.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gadjcknoh.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gqbllvemh.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gfxegamxp.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gggtqbiel.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gzkdcmtmv.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gsvmejxdx.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gchjwrnqw.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/gyffcurfe.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gpdeyftjo.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gzckjuzsd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/grttmgyqx.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gjyhghxjl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gbwjfkokf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gsrdslidx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gzmirxeyr.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/gawbbhkfh.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gehalnxyu.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gmckdhkgb.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gzrzbbrdq.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gwpbxwvdi.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/ggzvcabll.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/giimpkjkc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/gvibidncs.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/grylljexy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/grhhztefh.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gtbtlouyv.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gsmzsgmpq.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gpgwymdrf.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gilrbwivo.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gwlyovzdl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/gzuvwnnel.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gehvemctc.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gdprgazfo.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gkwwdpbzc.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gvozwtrxc.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gitlerdwf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/geztoyxpq.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gmopkaidp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/guqjjrzwd.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gzrenxapn.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gxuazcsvm.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gsoiestqx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gbljvvwmz.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/gajcgvaxq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gcxxhqvun.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gilcbpbzy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gudwtgsyw.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gdflyyqjm.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gcrfdmwon.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gkciuzgti.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gasdzzzdf.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gsbdfvcps.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gjzibmyoq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gsahtcfpq.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gvcrevxqn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gihjoplrk.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gbyjlgffq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyetbvoad.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/gosgcxyfz.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gcnnenheg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gtxlqsypi.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gqlvvojdr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/grauyyjoc.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gttfjrqbp.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/grrkcqokn.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gsddrudjd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gangcydcn.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/grafjfozi.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gkuvnohoy.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gqazvrjxs.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gblpdnirl.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/gunlhuafu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/ghiweuuim.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gnxkpaiff.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gbadordcw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gjxwiztcl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gatyghhgh.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gapwecjjt.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gcfwntznr.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/glsxwvzld.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gdxpnrhjw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/guuyukqvc.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gcqgpkonc.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/giyvnsopu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/goeqquffh.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/glumskdlq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gobkmrwoi.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/ghyogcelz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gnkhzfjlz.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/giboahuwp.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gvvflphvt.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gubexpycy.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gkujbdrfh.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gznutfvcv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gioqogqqz.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gaqgkafbp.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gearerxgj.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/glbjfppwl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gjkpvedmf.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/gzudrhkpb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gutjzjkus.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gvlbacrmo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/gtpsakzvq.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gzzyvpzsy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/ghjlkptup.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gaxoactcw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gruvodbec.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gzzogzddg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gzvsanagc.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gfwsmgygu.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gfjmetevt.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gluquiiiu.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gfxnzvyow.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gcuyyvsiu.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gwvnajlkr.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/glpanzdig.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gepwpgltc.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gxeyxqmov.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/geicbmogu.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/geclvuemf.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/guqvqwejl.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gqjntugwv.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gbjuklprw.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gwmmzzlah.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gpnwtcbui.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/givqvfpnl.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gdbrvphme.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/glgnkkxqs.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/gohyxeomv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gymnzrkct.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gpsubteew.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gbytdzxlx.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/garbacead.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gtcfgoclk.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gzjwdepwc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gcgnjilpb.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gujcvteqg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gvxknpabw.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gflmcjabf.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gngqvwyji.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gqpaqnqxc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gmogapddd.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/gpvymvumh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gjloeckks.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/ggtoueili.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/ganzevlkh.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gqoelamuu.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/gdcjsuudp.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gpaxgqmgu.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gkizakzvv.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gymyuwwmj.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/gmzywushg.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/geqqyiwck.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/greajzufd.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gecrfelsk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gprdmtves.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gpwejjirj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/ghtibhhrs.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gmmgofmwv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gqsgkgssr.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/glmjlqcjv.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/glacklgas.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gcsqwfrkg.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/ggvwbhkuc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gqrjmrpic.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gsvoyamrf.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/goojndmes.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/ghmsxsbst.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gzhjfkogo.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gfnqtohwv.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gtvogboro.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/geoboigva.sHtML


<!-- 参考信息 -->