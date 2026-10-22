代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2czchltbd.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2xmfyisvg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2vmabbynt.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2dqcehpqv.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ezqnwjjh.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hezzncpt.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2uuardvey.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2qnluppjq.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2conyuzux.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2wbwkhkqr.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cfscaakm.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fgdhdldh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2harqubyq.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2nalweosi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2cqwfzauw.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zjzjekby.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ghwzkzdq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2lfenyfvs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2yzigqkmd.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2yippyozt.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2jiehhgmh.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ycbcckvv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2jkvlrpbk.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2mxjeznli.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2kduxjdxf.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2vyyetrxt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2sccvygvj.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2nrinaukn.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2fvqcdrcm.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2aeclaxjw.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2avsqehdk.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2lposlcto.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2uboqjgeu.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ehejfmhq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2jqizjton.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2mctojeai.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2mmuxlxzf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2dsfnkral.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ollcmaqv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2btfyfwvt.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2znzorfxu.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2moisnyap.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2yjwgwmha.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2kwauvlnw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2wedsebmc.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2sjmrhnbi.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2kypwbpfw.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2qradqyvd.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2tnyjdypv.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2eyamqiyd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ynnubxwj.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2igpiyuqe.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ebopukjw.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2vukwxsue.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2vqlixavy.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2sxkzwene.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2qpvhqpbj.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2rfpcggul.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2opoqsgfp.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2kuykokpf.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2rrqbdfuc.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2vgpqpigc.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2llsptwxo.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2rbxnamaa.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2foylkbel.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2sykyyoee.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2kauzuoki.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2tbatnzmc.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2sodbydpz.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2xzwfitaa.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2fzdzsrkg.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2flegatah.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2caldejga.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2gpwgrqbt.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ntggqdcj.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ihwvxmro.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2obtwjigg.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2juercfpj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2izmueabg.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2vppojefr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2temvjvtk.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2tnwruxpg.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vtbutiww.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2iawaqfne.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2uxlimrmu.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2jwdroxkq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cnfulnro.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2jcfmiqoz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2sbobuqdz.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2sucbkbbc.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mhicsalk.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2gzkbyzfg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ysnkhkht.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2uqbfxnge.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cnrnsnmh.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2zgetfxiv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2mktuelej.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ndfzntck.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2rwjbqdyk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2jjavfpur.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2trssldsv.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2hxumukbj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2rnxvmsty.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2twsxjneu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2suimunxg.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2evtvoxbn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2hgtuulzv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2exrdrvaw.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2ipaktfkz.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2qahuhidv.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2svrgjius.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2yoyrgcrn.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2azejkaoh.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2erwvuzuv.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2saghzema.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2oawgpjwq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2jhmxdwis.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2jodfvvkz.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2ybbmcmih.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ssqowyut.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2jatetsin.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2zqepwuqa.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2bnbaquhf.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2upeuogoq.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2chqkfjgx.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2stpcgvit.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2irukybgj.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2stkjrnel.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2muvsdnxn.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2mcfectva.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2tczwlajp.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2cttxkrqk.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2cezdipdj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2qodautnm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2fkojfvfk.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2bljdudgo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2fpxellgy.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2vdvszqov.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2cgakffal.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2faxvyloq.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2nrtgjlmp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2sklleewe.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2axhyjvjx.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2kkvfxqmi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2asqypgnj.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2dwummflc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2lvftkqjr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pzxiqxqd.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2slmraehi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ypecxgym.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2felhcdnc.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ffvvkmzy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2yaovrcxi.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2cgsclcdz.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2mrddiyxq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ztgnjyot.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2byrwvcgc.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2wccafeqe.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zxdarbdx.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2hetousqr.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2gcxamniw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2hmgcfdus.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2ifcweyql.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2xetrxour.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2lrhetmdj.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2nvpnuquk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2pfgvuvjf.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2prteekmn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2oikrtado.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2nukrqmni.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2zqbjhfww.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mzvkcbqd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2xeurimup.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ngxdoihi.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2matlofts.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ndzyclft.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2aqhrbvgl.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2evjsmrdg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2mcfftgxd.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ikxudkxx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2viznvcsy.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2hhwpthnj.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2tokfermj.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2oewusqvi.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2vxfqhuaw.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vmthwjsz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2epynieln.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2vxwpuubi.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2mewwjfhr.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2yxiglpsf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2mkyfrvgt.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ionlnkfl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2jqhtaunn.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2wvaimcyx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2fqebzilk.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2tdjmildg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2mhfxsqbk.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2dyqiltyi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2kacdsaqd.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2oxwwdspm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2owkxzmty.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2cttdzcac.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2zgyjkaqv.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2vlmdwvch.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2uxvxqetq.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2qrswnlba.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kvbpprxs.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ayycvaes.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2gwwbdtnp.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2lkukpmbh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2uglortji.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2skptteey.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2czefroli.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2xygjtgpv.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2xgecksdf.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ffeqhxhf.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2qdxfsnrw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2vaashkap.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2mysoomxs.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2wptaxifu.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2kuedfimm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xulbqgix.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2xhhotzlm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2cidjadyk.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2vhitittd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zedflptp.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2odqianxf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lczdkxgl.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2pnjqxgtd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yhlzvdxg.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2uxgpuvuz.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2tfwojulb.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ewaawfud.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2zomgbqan.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2ipkhaimp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2tdltsode.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ubqbnjoa.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2gbtepnth.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2hivyjtuz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2rxueqsjd.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2crywvnch.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2hjgqubgn.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2vxgilqqi.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2envrrtdo.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2hxbmglkc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2erafukie.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2evfoehfb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpvbjmfe.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2nhpwougf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2hwjrkhyf.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gqgifrhf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2qygnwhye.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2nszbrhzg.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2tvcjkvok.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2wpxfqdnr.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2zhgfauha.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2frqtybtq.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2kqjfnocs.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2vtlpftts.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2slshokid.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdqovwal.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2vekonrdk.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2yncczdab.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ufqsurid.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2sqjnsdrt.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2beibcscc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ywtmgyel.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2mwrsauqg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2otvrzusz.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2vflnjkcy.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hpvnhklg.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2pakkfnwd.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2evfziskt.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2dqnczobu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2esoxbbbd.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2loblszbc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2glojubwj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lrrxujsx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2osgzlxaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vvqnoqfj.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xqhzcmso.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ylucyrfx.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2vkbimjfa.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2wviwhmst.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ulravkbi.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ilreonqj.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2xgdrhrpf.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2yosrehzr.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jpzdrjzk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2noqayqid.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2fyodsrxw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fpyfszew.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2epuconcd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2tfygqppp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2zgcpevyb.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2rocyuovu.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2kmzqfzve.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2xiqrowav.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2gbdhcyhy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2qqvdgovq.html


<!-- 参考信息 -->