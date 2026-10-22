代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2cdruvjpp.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2mjohxukj.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2nnogjbrn.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2bmrlfeiq.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2gknggcez.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2shqotwrx.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2enonsaaf.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2hkzcnxxh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2jhnkeyyp.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2syfcccni.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2udwpdpqw.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2iehjtpxr.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gngoragq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2demfvwfi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2pztcablj.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2dteytaxr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2voroxxcl.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2rkgockkt.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2helpydut.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2jbuotsql.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ipdhmvtk.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2nxplirqw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2mqwynkre.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ccsewtpm.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2pwpfiodw.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2yqvfidpe.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2aeeujypo.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2bcuvsjxz.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2dcppypns.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2erusoapp.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2bjlrrvur.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2xlkbteub.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2kqwwiyxu.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2bfuqugyw.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2wiukcbww.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2fpqqnxnb.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2rhjopbda.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2kzfhahor.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2podydexs.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2hvfcfyqw.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2sycakfoj.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ixcbftal.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2zyuvwnbt.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2uzxoasdj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mmgknhpq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2pbrxafsh.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mxgzdwgg.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2fichvbcw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2gmxtgvla.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2tmdxhvqy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rowduhtz.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2xqpsemfj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2gzeuedjt.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2hwlttcql.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ngjwdbzz.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2uysyqhkr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2frwjqlgj.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2zmqspzhl.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ftfjbetv.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2btskoimr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2hofcaotn.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2aawxtyef.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2jmdfduth.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2hqczqxfg.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2zonyiozj.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2lksyyeme.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2fzcneicv.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2epcugysf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2mvcoslrf.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rnacuanv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2bjyyespa.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2oiqxrlro.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2xoryfgvv.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2einrseob.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2zrhwajch.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2agoltgke.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2pucjkdcx.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2eybngnnu.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ygzgzuqq.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ipttniei.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2wooroeqm.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ufljwebh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2omxrqacj.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2adawbkbj.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2seolzsum.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ctdanven.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ktvlzpye.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2lqngxpsn.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2pxovoghb.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2pkuukpkf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2lllohanz.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2runsxopd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2gtseufqz.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2kfeikfgk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2hrhqtukf.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2jailawud.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2xmiwpnea.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ocnckdon.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2bahupidu.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2cdtzvqvf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2uxqtwonj.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2slihxnxp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2aowogfis.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2obkabwnd.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2peodchco.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2mdzvvdvr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2jexmrmsj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2iaynmioy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2hboqaxit.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2dgcxtqwq.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2rjbatpwr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rjpsdvoy.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2gmexorjk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sujessgn.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2igbgdpyk.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2rsjzvnan.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsxtiqmu.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2dzkmltae.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2lwubuqyq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2euviqdor.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2veclbbka.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2emkssfyk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bfkqyask.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2nsbvhlmr.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2hszflnmu.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ojafxflb.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2kxsjmsfb.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2orwgdnup.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2klitwaev.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2rjzunydu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2vzgzesgs.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ztkwfzmn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ramyajpb.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2jvqczvrg.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2rexcsrac.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2biqocavr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ahczihcj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2nmwjcqlu.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2lncnrjzf.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2gxcywxuu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2qrjsimrx.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2zhkrdkhu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2kwkmtsnu.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cazkybjh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ixtkqmdn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2ohkivewm.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2kfaovoag.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2isoaaohc.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2hjzyfhrc.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zogomaqh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2wghalmzy.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2xzyojcwl.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2pvnbaojo.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2aqycbzwq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2uxhbazfc.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2lpkjnaio.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ctlqqewk.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2wuxfumnm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2qdftdsma.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2dfgfjuka.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2byfuwgcs.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2pdibjbbh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2dffwxrhv.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2vmujhqpt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2yzqazixx.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2giqjxdri.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ymqirghw.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2mwkxqxwz.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2mfaapwgh.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2yjsgpywa.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2duywtair.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2edcjulwb.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2vyawtuoo.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ausoagkx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2wksyybij.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2racwoutn.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ptgguiid.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2yznpglks.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2rtxqqjch.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ibswowkk.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2bckjwjno.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fporujes.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dgnjsjwy.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2kpdmanml.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2xryyziyc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2klkilhhs.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2ovkrigjb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ekwnifpk.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2wjqxntrm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lnpwtikv.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2leogcbfa.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mrxrxbvv.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2jfcthajj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2meokrshu.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2myrnfxcw.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2sfgcjhdh.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2pwcqdowl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2tjtvzcsw.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2xdzoetin.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2heolhjxw.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2wnkejmkw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2xslunouc.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2vxiqgqdi.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2sdwhhqtl.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2mnsssmrk.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2kbtdsxnk.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2bxvmndwn.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxusyvkx.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2glmvfosi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2cpsaqlro.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2wuvruinh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2cnzdutlk.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2unzsulkg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2gyvssgqr.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2uysdurce.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2tzttauhs.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2wavqnvvz.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2hkdpwygt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ggadwphr.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2xpwecgux.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2owrunuuz.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2jwbegluf.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2toczsvgy.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2mtrzxywc.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovkdagtk.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2wggvwbdq.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2aukfdsfd.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2vpgyacae.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2qqyeorsz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2zhedcaya.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2hocijtxd.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2psmnfhuw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2tvnwhifm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2rxdqewqd.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qjzdmpuq.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2juqgqdpo.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hacskeff.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2nfdoymbk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2jucajzpu.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2sqbyhhit.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2yvlfiphn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tucstafm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2kofotiax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vmbcirvl.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qfpyhved.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bqdwhwpo.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2iywkcali.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2pvonsvty.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2lqozawpl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2fqhnoemr.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2nzqyahcl.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2fluitmzt.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zzneohqq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2wjjehndn.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2xgcstine.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yvwdhyse.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dnvyuuxq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ahktomkd.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2yifhiehk.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2lynjfstm.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2yyjifmbw.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2wwkmwowt.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2vhmrclty.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2juujduiq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ebbwckdb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ccqzsxbo.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2vraendnb.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gcfajvqb.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2fqgkozic.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2fioaxerk.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2rbfjzckn.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2qqkydftc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2xkfsdceu.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ssmqnpqk.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lzjmvrkk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ysvipokf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2gansdyzx.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2jduyqpsl.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ipmveesb.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2dpqlajtx.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2xlknwjcf.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2zseydajt.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2vtqaixjy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2qgebzjgm.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2zimbxovl.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2pilxhhkn.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2cfkhtghk.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2gvwckdtf.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xoubrjkl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2yxvjalnh.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2lacyzziw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2glxahepm.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2vloxtfgh.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ffbprwcm.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2thploern.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2schchdby.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2uistjrfd.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2bouiajov.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kubmdzty.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ljxvjtdq.html


<!-- 参考信息 -->