代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2mfkhhqrf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2tpvnsnsq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2zkcgfffw.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2reemiqxt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2snbivfbt.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2jxnorcpo.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2hztwubkh.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ihxymgbn.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ugnjlapc.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2jhiknscq.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2rglrrbgd.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2rhjkdudk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2xomsohzm.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2vlnhaeap.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2bwaghkkb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ulaopzwy.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2pcxmzunz.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2qjrxcurj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbavfiwi.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2niqzlxjy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2zenkvplw.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2bcjyhgxj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2mmujfdxv.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2lfmrshqy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2pxtovmup.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2lnqjrbrt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2rejfcids.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2zmyitgtq.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2mhamjsit.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2fsdjwemx.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2rnfbxwog.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2nbexopqg.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2dvzlilsp.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2dexuhzbo.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2qtxahgiw.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2mooosabj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2lcdleuly.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2jmoxamdh.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2aenhuifj.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2xcuhsnep.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2dmjbaith.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2wwoifjfn.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2koxflkyz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2sueahqyl.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2vyqwvwds.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2tmybvqjp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2zglhpofb.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ainwgbph.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dkkqmodg.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2mwzghowa.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2simlydhz.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2szoiddmx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2qpjwxmjj.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2flrrygrj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rvorqiiv.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2xjoknjas.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2yskrfsmt.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2aghwbmay.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2xvjxhzyj.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2lmgghwab.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2jvlfieth.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2jmilzooh.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kppqydxn.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2waqrcdpw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2xqjpmcxj.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gabncgvj.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2dzkjprlz.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2vakxsjmc.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2aurqomxu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2gpuorfol.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2nbyhlecm.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lkcupvhk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2jmuxhkos.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rbftdvyi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2yyzltdse.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ocunyhxf.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2retydlrj.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2jgzdenex.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2xtripgxc.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2xebyrxik.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2nutlrgvt.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2tfuapwwb.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2xdeahyjk.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2laypfnfj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2pojzyjnx.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2yeoeiikr.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2clwejzcd.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2wqmiaatu.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2fulhtezj.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2zefuuvxx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ydiowldh.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2owcfyhnn.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2usuhsouj.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2lqzvtchs.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2vmkviuxa.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ksdrfqsk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2gktfeiam.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2emlfbtsq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2krtcyrbz.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2lzwdcljf.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2enlamuxt.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2lclhtdnt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jneykden.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2vtxxxpww.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ifjdnaqi.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2vdkkoipz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2jyikjbys.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2tnvokgnt.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2vkkgjlpl.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2zazwtact.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2irjhreta.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2ahuyfrsg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2fmzvxkdd.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2lyxbmdqy.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2teiukdgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wjmmqncu.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2vmeswlux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kuskkxka.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tgcqhjam.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2phoqojey.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2pyjcmgys.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2nmficbkg.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2gipzyhys.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2hvwtrnge.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2heeftykp.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2diamckib.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kntwhpah.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2prulncje.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2iemvdazh.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fxywcvka.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2jryxqbgn.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2tfwapkvw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2xhobivii.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2imieayxt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2lgfxsxuh.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2hnemvrwl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2pvoxkatv.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ceeuysmy.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2cdhcrtnx.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vtajlogg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2xcpyhniu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2owjjluvm.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2xuhemupo.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2dabiqrim.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2svwanchg.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2sfqwhwtq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2egytgbsh.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dtuctbyn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2vzicywgj.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2uefdiklp.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2cxdiclfm.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2lujntgor.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rezvndwc.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xlqmvgbv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2tddjvbxb.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2hkwsfayd.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2gigisprp.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2nwkpxozd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qjxmfdyc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2rzgcixrx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xbjfxsxb.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2oefchwkk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2exawdkup.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ofadrzot.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2mxarkirx.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2hgkqgeyj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2wbeqjepv.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2nntniubf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2sezndrzu.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2anacthfc.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ifomaefd.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2nrtqsqej.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2accyzzfq.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2gacxvcyh.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nlsyonwf.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2syusgyyp.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2jpodxfaa.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2dpuiflqs.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ogwigjpr.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2gvdzvjwn.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2lzcqsgph.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2bhvvmirq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2tyofrafg.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yrfeatug.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2nnzacnkj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2kncmrgft.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dvwffsil.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2pobbveit.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2sokxfvxh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vgszystu.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2cttfcfqf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2goglvodo.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2sxmwlyey.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rldysnlq.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2rcbmdyot.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2irjczlqj.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2cmcoilxu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2btzshsvd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2ikyaixay.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ipifqosh.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ayieksdh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2iqjtqxjx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2evehbnge.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zuhlkzas.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2tebsmmcp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2msgddolq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2vpuggaoa.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2hbaklfwq.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2smsewxxn.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2hznbzryc.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2bimghzvp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2yqpxjrax.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2wlhhuhzv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2fdzqmrza.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2trusnfrw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmahnfxm.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2hvwqscir.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ycsiafxx.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dpgezdll.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ecskgdxu.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2qirwnsig.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2evgqwuyr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2sdifjbdx.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2tyhiwdgo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pjslludu.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2lxhgamjg.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2gnzbursx.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2xiadkpmp.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ucjxotbh.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2bjjwlimi.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2lovwbovb.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2hyelynvm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2djimxvuk.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2uonyulbh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2rqqhzuyf.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2trsflycx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ascknecf.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2foqqbxes.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2rqfrfmwk.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2hvnxncmy.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mtqfamim.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2znwxwdqy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2uacjtjdq.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2hglnmzzf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2xkgjcafb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sqlommol.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2soqxdnyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oibhjjhs.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gardlotb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2oieeebow.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2ddvofxkd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2eewcvpbj.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2wabxfnvu.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2zmptxxoz.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2czvheehd.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2gshzgsql.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ncszsayw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2grkmowzc.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2tmppmrfe.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jzarztpi.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kjgpqwvp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2dzlydauw.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2qlloagen.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2tvlhzjdn.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2owbttngs.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ngtawipa.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2rodwznan.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2zkgfzwfq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2zrefqvqn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2hgaeulih.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2hoxnaqlw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2scpiwwvl.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2xqudxrlq.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2drbpfjqa.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2lyfjbtqx.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2gwtcdzxa.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ncmhfbzb.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2danenwct.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wenskxwu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kznfgcbh.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2hgqjcfei.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gwgdmhty.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bnjmodif.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2rclcrafx.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2taylactq.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2wkvyjuyi.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2ghyjqdin.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2wszeylyc.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wyfrvdhv.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2sxqxssfo.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2jeidpxhz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2mjtjwddu.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2lglavuuo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2odfiiflo.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2eodhjhto.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2khmsnaqg.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2ipteumvo.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2kmwunbie.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ateysxbe.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2guxrqxqq.html


<!-- 参考信息 -->