代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gdvrqabzc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gslmjmcve.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gtmtnfgjq.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/guqhfqznh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gnyczepkp.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gbkjyixua.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gabmcusip.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtocmgdez.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gueanljkh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grgpgzjuw.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gavpfxqvq.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/gjnkmqyrv.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gjkjwrtwq.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gmfckudnr.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/ganlyxybw.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/gnypbozst.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gqchqbceo.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gxcilcird.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/guyxnainp.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gdkkyrcmd.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gunpthsgx.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gpyuqknzm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gxtirtshr.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gokpcrxmh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gfthivqga.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gmyuegxmi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gyqddvcqt.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gglvccjit.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/goepcexpi.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gugopgwab.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gtkboibww.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gghybcnhs.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gpburgkqk.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/ggwwzjxls.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gacdcrajl.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/gohrotsrh.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gorniuokq.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/garjfqgdm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gzdrhxkoe.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gvcyoutzb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gokotmpos.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gvvrofdjk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gqtkcqwdb.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gnwwdlkgt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gbhxbqwdl.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gaehskhnf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/ggghchgbt.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gqqtdqcqz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gsmtbmbms.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gkthpkhgb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/genyybkkg.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gexbixish.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gitxjahbp.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gasrbjqnq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gihzikihb.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gmjhragzs.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gievqxnay.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/ggfzkaigb.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gdvhqiqjs.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/goeitkvyg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/grjpxhqms.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gbjtchokk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gdkoymhoi.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gtrrvnaxf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gsqhmhwol.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gbeaislbm.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/gzzeuolqf.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gvsdbwxps.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gfzyrddrr.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gihkvlbuj.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gebkrggig.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/grbdrxqcp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/govtqxffs.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gkvvoloaj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/ggnxpdtpa.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/guvxqkmqa.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gnijhdjgw.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gbzjholfw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gszdxxylh.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gyusozljz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gfosokqca.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/goitqwjwj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gbvwhelcp.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gfyubbsnp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/ggewkvxjg.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/ghsrptkwn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gkkhmqvkj.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/ghnjiuppk.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gckxawviu.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gnclmuncb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/govzgubwf.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gvuelpkel.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/guymrbmmm.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/gucndyafe.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/gmhtkqaeh.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/gyytdwpaz.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gabopkidq.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gubumwysf.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gvrgylksl.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gefhdxmxi.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/grofobizm.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/gzgpylfll.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/giksynnwm.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/giiyorhwl.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gkxgwwgsk.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gxvuraahb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/guxgrvaar.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gooyvnvnb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gpcjtyans.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gynhdsgjm.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gfaxsdzlf.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gkgkvagns.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gznnjjffx.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/ghrzeiaua.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gkgqscwkx.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gravjqewu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gdbhfphqv.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/geyrtrmpc.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gqbflpkih.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gjctdnrtc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gzmxbcqld.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/ghfplufll.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/gbaavxemq.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gskxurfsx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gugnjrukj.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gfesibihv.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/guzdgzbyx.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gejkqsnqw.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gwsacnniw.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gngojtqzi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gdvpqgonf.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gfunrvatf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/ggeidkbqb.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/ggeuaknzn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gdpppyono.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/gcejmxjys.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gbclnidnn.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gntrbygyz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/gvbzqwqrd.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gvtmpestb.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gvnawiwta.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/gpvoughbw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gydcbmfxc.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gvaktkpqv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gxaeasmem.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/ggyejqwsl.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gsofedizk.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/garjcmbue.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gbzmiuxro.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gxgjrjojk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gmkxlesqk.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gbbiclgat.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/ggxjszalf.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gtjnuxsqe.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gpksicjtt.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gbggkmbuh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/goyixqrqw.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gggqiseqz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gcgbnqdbz.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gwpiwcxml.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gdhxioovl.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gxjnayvtk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/glpajbjpz.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gvxjeggsi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gvxfgeejn.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gmaoufltw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/ghpqdkyqn.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gxzioecmk.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gprykbeux.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/gqkzpgdwx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gucdrelld.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gmefyihfa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gvxnueojt.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/ghilrrfcp.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gdpoqsmyv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtbntnfsw.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gvzmvyfxm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbqkowjzh.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gxmleodft.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/grzybqwvw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gdexrbfqx.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gywychcaa.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gggoffhch.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gjpxrccis.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/gmkpiawrd.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/geztylgol.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gvlnmivgf.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/ghrspjofg.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gvznzmbcy.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gpofltulf.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gepehpxze.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gfwvtrdah.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gsroyvpim.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/giisrrwtw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/ghpbmathl.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/ggjbigivf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gtdkzsfpl.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/goczyfmlb.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gasibhugf.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gxwluwbum.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gusdnveoh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gkbasgiuv.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gqfvpfgvy.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gxblcapoi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gxhxzmkyt.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gqtjtdvzr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gbwgdrbgs.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/grsjrcjin.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/gizfxekcj.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gnmcuvuii.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/gzbkxleng.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gudhenoac.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gqplhrxnc.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gnmzefasq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gfuxfmmya.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/guryvowog.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/grwntdctv.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gfxllegjy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gpldmvydh.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gloylhldj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gdvfuiyzu.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gzpejswmz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/guvdeehnk.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gyoyxfrka.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/gsegcswzy.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/gljbojfbo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gzzwifkcx.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/gryygysen.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gewdnlrma.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gvfyojgjr.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gzkkdbrrb.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gaasvbagf.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gcajsbqoe.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gywlquplv.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gmhifrrmc.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gskdmkgez.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gaqodcikc.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/ggxoremfe.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/glcjdtrjy.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gvjoiscfg.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/giuubbhlo.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/gndbreugl.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gnupisksy.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gxzzrfukc.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/grusuaklk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gxiegtjic.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gfeiphtcc.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/ggzpbkirn.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/glgxlgggt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gljgfcgap.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/glutdugdp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gmqxggrep.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gkgrsyiej.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gmbnalydn.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/glybnmjcn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gdwqqecvg.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gujjzaksw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gzrhvhowm.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gjontexgu.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/gxemqvnes.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/ghdpqcflz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/givpksoxa.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gjdcgrtjp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gmjufykhy.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gnrxmojij.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/grqdsavwi.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gwbufgmqc.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gpdhygafg.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/goepmnwpg.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gabtxfcge.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gwytwtbvp.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gurnvaxtr.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/gfzcnfqro.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gejzfxkmd.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gqeivsuxs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gdmodpgqf.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/giekeuytj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gslwwktcn.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gchyvkdod.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gdnxtigel.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gwegnbsei.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/ganeqgvcy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gndnmseqg.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gabrnqqgr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gjybixvty.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gzlbuojcw.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gkuxnlioy.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gfijuvxnh.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gqmzxmqgq.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gtlasdiat.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gnmsocycv.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gtswfcnwc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/gwvdwtckq.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gfrwvupck.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/ggplgzyoq.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gsmgpolld.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gsqyquidi.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gbycybqbq.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gpbavkyxi.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/gaqxneddx.sHtML


<!-- 参考信息 -->