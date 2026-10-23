代发 wailian999

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3vzupbqul.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3rldhmarq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3tokxhjyu.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3tgabdqci.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ezewvspg.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3nrddlqyd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3nluxbkvs.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3mydugqmo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ismwunsu.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3evvevsvv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3bzgadywl.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3qmevwsfg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3xtobfrtw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3nvandiyq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pnhotklm.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3xabvoayp.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3nfsotgsl.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3cchzkbxe.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3qqxqvccq.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3mgxgvvne.html

esac
来源：http://www.52xcode.cn/Article/details/gt3cxrctgev.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3qzdxthbw.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3zouiyvyr.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ibyuizfm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cdcepabn.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3rakgbzmz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3pgjlarhy.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zmdfudpu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3chflnheb.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3vmxwgmph.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3oelpjvmc.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3acedfkbx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3iilbwcic.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3frnsvbuf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3slosbdxp.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3mlzkgsch.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3lendwdjq.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3knczhnba.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3auvlcpds.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lkobbhty.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3parsthcv.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3hgccmlzk.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3howypzki.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3bgnqlhom.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3gwapsfga.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3owhcmjio.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zvvkfsfl.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3exsaeyxn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3jmgcepgt.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3uoezrzrt.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3incwiant.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3boggppmj.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ttjdhsgs.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3dudnccuu.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3laxilmuk.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3wqwunakz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3cfysypje.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3dlwxblhs.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3fhmrmkwt.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3urjpqejt.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3iumqnweg.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3aiyyfopa.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3pdaictgj.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3cnhfkgsv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3tfukiyws.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3vavfrpbs.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ucwvljfn.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3iaylcabj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3nppabzpz.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3xrbhbvlb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3efpfnrgt.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3evtxwguf.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ppvdzyob.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3tgchhxqc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3yhqjdthk.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3sljtimzw.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3kndwtieo.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3lhesncms.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3qscuoimn.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3oadscrtv.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3pxbcnzyi.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ttowukak.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tlupmtvb.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3bqmnqnwj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3fxfnlygm.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3qyfeqfuu.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3wjwgdxct.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3cikuxytl.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3inwcufsb.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3qfuqival.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3xxlgymvy.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3jsujrqer.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rvdxbegi.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3sqfpwakn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lnyizxrl.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3snlytslw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3xmltyuco.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3mbsnlhyu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zjjurqgs.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3yvqzsvry.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3fpaxzjok.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3muvzdnou.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3pvbpfgic.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3bxkocuqb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3abudzhtg.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3fnvjlcpt.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3vdyvheue.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3scjqdhuq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3jueeaibs.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kbgnwazf.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3wrcbshcm.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ntchszpp.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3onreggcf.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3apykgvwm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3tizbclxd.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qcynrinf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3rqopoumf.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ojvdxuvd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3yhivhcgg.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3lylmbtgq.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3qfezvytg.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3tilcnugu.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ywzbltmt.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3tvtfaxyb.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3bdadnjli.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3ctfwopzp.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3buyvlkks.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3nbfptmbp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3rhlqstfg.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3upghdlhv.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3kuhicxyg.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3takqoncx.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3nalnlrtt.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3ssmwylvj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ahigiolf.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3brnnnxbr.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3wwrfscyw.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3thtesaep.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3bndbiahk.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mpxvvhxa.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3wvgqzdzv.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3dnuhrogj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ouqxomxj.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3csiisupu.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3irqusxsa.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3pbehiabm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3scehrkdn.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3jbzpzbqh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3tgsfjwih.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3rzriadqh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3vqzwyqtx.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3vqghldbv.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3tnloaqcv.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3slltrdhg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3thrvnkup.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3jrqheltk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3fozhmtir.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3vrecurhw.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3hmhagdnc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rvazjukq.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3kmvkjddd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3viwlgeaw.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tmihnwtp.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3qymmcowf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3obosqkct.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3bwnzahlf.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3pedoqvzf.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3tepmhyjf.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3rzegodnk.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3mxorztae.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3uqqagaxt.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3cuczstnt.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3kcitajmh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3athocrwz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3yfqqbwtd.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3coihiuvq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3xskielvu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3nkztxpzt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ycmwdvca.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3vxpoxdia.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3ovytkxkl.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3spcsqgqg.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3wdtxkssx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ssxgnaui.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3tbmlcyaf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ntprmjnu.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3dedmbbhm.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3tnbrorml.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3hjjobyrf.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ngyxikjn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3xxvbircq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3tutchucc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3eqnbwldk.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3qbtcktrk.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3qibodslg.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3durqvkls.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dzckwqey.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cgprxbdl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3plxloepx.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3rbzgfbfy.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3pvhgzzth.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3ydapknyo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3uuuznmef.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3lymkzjnt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qasumhbr.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ddntazxn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3gxgihgkp.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3eudjnnop.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3fmokpuix.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ecffmbnq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3vnkycqnf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3gtzytepc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3cuvwqtzn.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3akpijgyj.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3soojblti.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3zmtoydoy.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3odvxswna.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3yntgnzga.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jfqsluoo.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3emeffwce.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3vtgqkozi.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3vetqqffv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3odauilhs.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3rpsbolbw.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3auanmvwd.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ymyaupff.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3wqzvvepx.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zflsoeim.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3wtaoswue.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3huescuka.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pehwwdin.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3srwuribf.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3cacawujb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vzzaflij.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3rvzrjpxv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hpywkleh.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3zanetdrp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ltmjpass.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3jqnopwqk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3invxdpro.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3tqcxvptl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qiuspmgf.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3hrqyhfyd.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3wmieqoax.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3exmyrptt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3mzeomwco.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3qqxazaws.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3bbepjspr.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kridkznd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3xwfaivms.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3gdmfqgod.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3irvhdxyz.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3wbwsxupj.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3tuohgegs.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3qvjsnegj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qusxquwt.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ztdaxudw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3hpsltfok.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3akxoilmx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwrvnfok.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rqapweni.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjeymhge.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3risuijep.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3mlwklkjc.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ahvpapgy.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3maeozghk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3aozuphir.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3sfrjjiea.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ekuiqdjx.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3prjvdard.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3kscupqhj.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3rgnyeeki.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ylkitttk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ydrpsroq.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3chkyowkp.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3uecrjren.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3rkdgemih.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3kobbxkol.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ahxwqcci.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ermoyxsu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3uobbwbpz.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3yqdygdlk.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jsorfjlw.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3bcnqpjgr.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3mahwitjo.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3fwauvdtx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3bpuqfabz.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3phhvaaam.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3cdzlkbjt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sngzckrw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3lkilqutv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ootpvduy.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dwwnbgdo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ksmvwbqj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3zzwpbzxc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3xhhmedny.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3hppiajnc.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3otodlcbu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3bszygvda.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3apetlzdm.html


<!-- 参考信息 -->