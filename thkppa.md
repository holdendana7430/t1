代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3wqvjifyx.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3nkrlzfbs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jjcpnywr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mrswiope.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3jdcrhxev.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3vjqdcpja.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3nsoerupo.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3azzzeeoa.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3pcwyruyn.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3kbypaxkd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3pthabajw.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3zgtdvzsy.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3apuabvcb.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3umhmkreh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3afuymgvo.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3gsmyynlt.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3gcdzwxao.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3auwdczwr.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3jeqiqteh.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xrehnugu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3wrscapur.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3zsxuhapg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3avbdkpiy.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ndoxklfp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3bytmaejx.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3xnobythq.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3kweaglso.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3cgghfaaq.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3jgajgfyn.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3bdtdmgoc.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3gmcapuzn.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qqdhirun.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3nclxzawp.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3dipauuab.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3yfpvaqsq.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3jrqnnmep.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqfnubkr.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3vqnnmwnx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkloqiqa.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3umoiuwzu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3fwneniky.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3yubfqmwd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3hdkpcmsy.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3qiwfmqwt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3vpqqqdzu.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3olpouiwn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3obrpmqiw.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3plnuzdnj.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3yjspeubi.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3fmkddapa.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3limruyov.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3bkrxtzeo.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3kxzkrobq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3bakhkntu.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ilywgrsm.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ohdwjzyb.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3wjhikztt.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3nzszhzkn.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3akioiwvl.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ioyntvas.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3chkfcbon.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3thmkhxuw.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3vnydgydf.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3bxvibvak.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3agbigxok.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3wpjkaqqb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3oxligsmb.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3mgrzcvhl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hlgellxh.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3edhedaao.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gmtpmidk.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3uflyftgo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3fswkkltq.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3swjeajsp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uqbmhdew.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3lpaecsci.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3uxvlhkvm.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3mrwzodsx.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3rpkpxqmb.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3jynxvhjd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3vrkqcypg.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3qlzganmn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3smioozbs.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3wfdqozkk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3yhdabhks.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3fchqcvrs.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3czsqixlv.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ykwnzmjx.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3tqsojmbb.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3rxuorsjf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ooouzcas.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ruqvwbar.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3fiswnhjd.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3esqanwbx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ibyuxzuj.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3plmshpwn.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3btqwlfzk.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3hdltwadq.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3dyfyjiiq.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3itzrilhq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3hwotkngy.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3mogqbgim.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3hyrvdspl.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3smkucfgu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3cohtwljk.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3varwjymd.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3bkvcojel.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3xxlnyuln.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3tsbouzoo.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3selthwut.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3uncxfidl.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3rkqlvorw.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3lpseppvr.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ateulzmf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3vxhbhymw.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3nnrvbxlk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3okvrephx.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3mbkwunxu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3zcboubeq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ypzomtmx.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ngdrboer.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ouzaxvdc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3umqwpjfn.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3bsdejtzi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ogiirdda.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3djpcmbvd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3nockznsx.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3bmywwyho.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3vihsyphy.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3yhnjqweg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3afqvnhfs.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3beapeqha.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3oapcvqra.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3nnoegvwc.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3oqhjrgwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ovqbatcl.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ixbyttyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kkqolhxs.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dfghuvcf.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3wfebmrfn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmucfmql.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3akjdyhlh.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3tbqlerci.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3btvdbsrm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3kydsjowj.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ykwhtorv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qawlcylo.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3goyuwtzx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ghkrpqdf.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3oolwumdw.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3agionokq.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3raiamows.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3visxamef.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3fgxvjysg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3hzqinuxo.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3jfdxfvrq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3weectqpf.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3bjotbdjq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3numsqxnh.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dgosbsai.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ekfujtnc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3zjvhhycs.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3hytcvpig.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3jjnmljsx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3suyyhtfw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ipuklcmj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3jcmdzmpg.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3gcfgzwrp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3xjsttecy.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3hhlulmzl.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3yrprurio.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3fgzuhhbw.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3clmymsmk.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qmivnmbl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3redilgzv.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ulqvyuyh.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3jjubvlap.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3vtarwqsx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3fdniyosp.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3kskkikgr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3sgvcwzsy.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3jysouefn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3zymhfase.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3bthnubdg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3uffuwvsa.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3chfprlyl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3jqbxnpks.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3qbrasfta.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3nhzklfwl.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nizhgaif.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3pbriuqqt.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3kuwacnqk.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3cazrujyt.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3chlteykc.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dzobtcxd.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3pwyivwnd.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3diprzths.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3vtfopvkn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3dqewcyfc.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3zonkcbml.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3tukfgrjc.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3yksmfdpz.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3vpyksczu.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fwejeonc.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3eagpuhhd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uujnphoy.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kxslqxby.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3ostpilus.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3cjwxxvif.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3sfmgxdws.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3gqejeqeh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjfbwpsg.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3dqfhlhso.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3opkqgmyn.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3gggvxets.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uiakbsjr.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3vegeoorg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3grcnfpul.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3fjanhqrm.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3hceqdxrf.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3tksifxiu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3arbtwlae.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3gqaktkqh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3wuwgiowb.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3yiacfwaw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3qsfezpma.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3wxojqiwu.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3jnwtqbcu.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3yjtlwrlu.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3btooqgsj.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3gohhymyg.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwruuzux.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3rbynmfmo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3lupjdwgo.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3zpxijlno.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ckwkcuif.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3zxylhzxe.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3nywisqbt.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wrcdkans.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3oufrurzu.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3myuoajks.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3tqykshsl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3vneoyxce.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3htxpmcgp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rpyyrszo.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3tlwvwena.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3nsgauklg.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3kpccmdut.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpvjqaie.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3ormizhwa.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3gcenpiax.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3vwpuchvh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3tqqlcsvg.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3vfeukpyz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kevifswg.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3qducmgbl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmhqdrvf.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3ukubytne.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ppuhiuuc.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3plfpeupo.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vxiumdti.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3dskkkadd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3olycjylk.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3shjvzdjn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3zwpnntly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3roazxudu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3oqazeosi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oekaejwr.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qtdnuoiy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yfcpcacp.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3nujretrk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3rfbzaldd.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ustcixdy.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3xgqpojrh.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3fcffxsnh.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3nqknqwpx.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3iwqrkuoi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3bqtwijba.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3gxvhpypc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zdxlsngd.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3gdbznyly.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3mimwodlo.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3suwubatr.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3snuzbuzv.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3iircnvfl.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3lkrcroev.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3dmbwnubz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3acweluyh.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3chtrbtoa.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3qjoidbzt.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3aoowmkmq.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3epadpjft.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3hywbdqay.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yvjohblm.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3aguzonfx.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3sbijjtvs.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3fdluvadv.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3qjwohvht.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mqhwqfmt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kwzaqkge.html


<!-- 参考信息 -->