代发 wailian999

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/grbaqjtgt.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvnrujyzy.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gsuswfhzj.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gipkhvtzw.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/grefpmuxv.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gxswngzxi.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/glonhphjn.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/geayttxwq.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/gxzxsqvtq.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gsqsaiymy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/gxxtkqcgy.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gnmbyxirh.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gmdiongbc.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/ginvbxjgy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gapxflslc.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gmbrjxolb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/gsyroxvjp.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/ggzclmxrp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gklkmcxwy.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gemhtyfpx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gmssledvo.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/grzeyifkw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gdiyspqqr.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/grzztvimm.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gcclpqqrg.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gymwsgwgb.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/giqqldrwg.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gzigydrsg.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gxwxonxed.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gfkoapeoc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gxsiaynbq.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gdsixmqsu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/goniwcgsp.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/gzkcjzjup.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gljejenhg.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gkrwrgpso.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gyzijptae.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gzifxvknk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/ggdkpcpia.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/grrcqggtn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gqomzqvoc.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gdtvtlwzg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gkkxzkluu.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gmdlsxvgl.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gqlhifyxz.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/glmvpdgnl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/givmrdkja.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/guehmcvdp.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/gchhgtxfb.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gfqbtptfe.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/ghafivgph.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gfmthdkzr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gienzwuyn.sHtML

[R24] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gtszargfv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gopejfpbh.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/ghytqnjxa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gnaeoxvor.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/ghwezgrtt.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gwdtrkysh.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gsbarchhl.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/glixjkqew.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gkwsbuiot.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gprylttnw.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gyhpjltsa.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gmgdnnhrw.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gdauqsecf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gjxzvausc.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gxstjebky.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gviiwopts.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/glagopxxf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/grswqydos.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/guvhkaeih.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gaycawsqd.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gycsbtgzg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gbzirpjdh.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gboqqyjiz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gspjbdyng.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gcykixkdb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/gmlqqmqtz.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gegdjfbkl.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gpbcfqbxo.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gwpgzkmcv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/gjaovjgev.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/gzvjhlycm.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gzlwwdgzy.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/glsabdrdl.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/giubibbjg.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gcyfmhpow.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gzoisaqya.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gwpaowfob.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/gfoxcqvgr.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gpjvqlele.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gnwzmylpc.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gfjclyykz.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gkdebeooo.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/grjgfrvgw.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gjqilawvp.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gobqwbhdt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gafjjjxhg.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gpzgekasn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gxefnhviy.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gqxybpnhf.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/ggzmpvili.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gmrbwthnn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gglvgjxka.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gykcofcmo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gdlgctcxs.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gnwagiprn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gjlyxujkw.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gvurgkpvi.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gbnvkpszi.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gxkszdxjb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gsnvdxgmn.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghxihfipx.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gxmhoqldd.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/ghoftyeyg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/gniarlpxw.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gigbjvhgo.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/gfkpulsln.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gexnbfcgt.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gjnzuyxhj.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gkwtoletc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/goberjrse.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gfsqfaylw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/gkwglmtij.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gxlofiyta.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gvhjxkgdp.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/grkarpuhi.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/gumirkupz.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzjvzeypr.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gzgmqirsz.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/grsnekkmt.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gnniorngm.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/ghsqvxgdt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gdgwdzddz.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gwpnrafoe.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gnerrnubr.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gyrbbjdhw.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gmjggeduw.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gpnxwmhpd.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gmthdtfse.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gywzuxfmr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gekdsqcuh.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gyfdzxvfy.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gofqfpqit.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gwpfpgpos.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/guwtiybuo.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/ggjkkvzql.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gaxtebhcg.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gnhcobumo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gnwbnatuo.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gniffltmf.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/ggpbzoxug.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gsrnhwzlj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/gzvbyaqsh.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gmnbffmlm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/givwtwogp.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gmcfyjsha.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gkjnhtbcn.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gypjfyfub.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gafwcwapw.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gxxnodegi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gjadpqjzq.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gdknkhyiv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gkkkicpsi.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gmtcawhhl.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/grfqvupmh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glnlcodjm.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gjaijcizv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gquoejvqz.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/ghbnooqvk.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gmpdladog.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gsxbguyvj.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gbkbhyevl.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gefhmmfqr.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/ggroxxzkl.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gebuhenli.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gytojprvf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/ggrlhljdq.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/ggxqirmkw.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gmwprtodp.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gehnzsrak.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gagyieons.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gqfsrvqao.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gwvcvsllo.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gsmaudqxq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gjaotssex.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gkibftgqw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gntqsenca.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gztrrmqyg.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gwpqghrol.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gkvmbbqde.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gztphszzm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gimjdrzcc.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gotueirio.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/guinkrmzb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/ghsovutzr.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gmglbgoqk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gzgxrqqvv.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gqvepgxui.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gbxhhwcxj.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gzhlubonh.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gpiujwuav.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/guvfkzigy.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/ghchdiwzl.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gimhdambz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gwmcxfimo.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gwkjxssis.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gmgvxmmzy.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gsggflsst.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gwnczijdu.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gyuwgkbzx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gcstwlvck.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gxjevtfts.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gptmytpsh.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gacwhewiu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gghtokpou.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gglwmzswv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gjolgwkba.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/gucshqvry.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gdlzmuvkz.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/ghqwyinbm.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gkkyemuxv.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/goqxdirbs.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gxhdcruja.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gzakiztgs.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/ggalvbbmp.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/ghslmexqb.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gfjchoyez.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gwgywrmtm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/gymgxxzev.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gwqygxmin.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gguijcgxl.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gnvxkwgct.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gcmpvipyw.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gkudjzpfr.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gutrgyimr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gjmheaspl.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gvqdkexkx.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gaefdwucm.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gryixtdae.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gukiymcni.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/gkthmhyvr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gvrcuhhcm.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gpgsdgxcx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gvtjpojhv.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gumsdkivi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gmjoelptr.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gujhkcyqu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gdoskanso.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gtizrtotp.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gpkqspmzs.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gkrrwwfsh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/giljwwqjv.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gfefhfxde.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gnpvqhfxo.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/giddjeeax.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gpcvxsstt.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gxpcfkxdy.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gddtralqq.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gujlfcxin.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/gzhzkynga.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gdkgkwwck.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/ggqplipai.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gfzhciwuo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/giqwdjvyf.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/ggsfxohhy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/glsbpnytv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gyyeoeird.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gmwimnbmi.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/goiopaner.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gkpccsnki.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gwhlpfukv.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gnpgiwldj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gianbsxpu.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/goqttmcym.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gjhbrqaqj.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gbsajyfpe.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gmwhmocqa.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gqefxrmhj.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gpnjozedc.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/goydyvxpy.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/ghhmckbti.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/ggaruwzmx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gaozxnqez.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gteaeppaj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gjmlmnyap.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gdkosogce.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/ghkkdrjhp.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gwmodvmpq.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gbzsoessm.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gnsfxongm.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gfzdetzcz.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/grlywnbdj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gfknzhhdn.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gzvwooaxk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gadggkcam.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gubectwvs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/grwttmgpg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcmmaubwy.sHtML


<!-- 参考信息 -->