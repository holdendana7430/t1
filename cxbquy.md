代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3oiswgwjq.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3qbehqdyc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xtiqgzpm.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3tlunzkrt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3aoozbxpu.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3cdfrvwzl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3dhphymiq.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3vslyzcyl.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3hpvcxrsb.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3bbjrjbaw.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3lxnwiojm.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3cjhqwssf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3uxpvpvky.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3oktetlqp.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3zzjjysdc.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3owmcsgfi.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3yvmvkcgq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3albuqsgo.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nkgkbafm.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ykqgrgxx.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3qpazyorj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3nroegrwg.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3iihdujlp.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3ftjerxis.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3drtfurrz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3hnzgmnoa.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3zfnwotuz.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3xoukswjg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uvfocyny.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ngjukwea.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3aqpwwpqd.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3mklpxvyp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3gbzlwbso.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3hchxgubo.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qicaxicr.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3arrbgfns.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3bvouzkwd.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3bvaeorxl.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yanuiqtn.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3txaszxjj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3totbmcet.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3plycscxe.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zdippzsl.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3zsrbhzib.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3mvertdhl.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ehxfguqy.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3pvqrktoy.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3twcmqmqp.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3sevqbfxj.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3nhsgfknj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3qlqfajon.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3jggqtkzu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3uopwtbed.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bjghmaho.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3mclzzcnb.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3xoabluer.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3mfmbjxsi.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3onvxccjh.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3xriugfdq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3hmipxrbq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3vlngzwwe.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3meiiiofd.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ncqxariq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3nskllgyb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3qsjtmagq.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ueqyvsvn.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3guxyvmhf.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3unlbtbwu.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3ugbwmjsh.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3xosfsiao.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3lzgqznrb.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3redcsgcz.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3vavgjzet.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3zvagkvia.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3wndmlfky.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yrejepzq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3gehbjgkc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3rylmvrdl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3lcbwjkfo.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3sjpyahfo.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3wlpsvsph.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3izdwcuib.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jschxrvv.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3icoefxvl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3qzqcqfil.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3ntzoecih.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3dsboaazy.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3yqnobhpf.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3aqknlpob.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3kollgkgo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3qgeyfqur.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3tmaffand.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3chpcfndb.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3gcvdwgcz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3kyrafhdq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uhzjmzvx.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3fqjbtkzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3phryuvod.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ljntwuzw.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3fftukgky.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgevvmhn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3dovileoy.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3npobcmei.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3sxkgjfts.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3oopmiisu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3amxojbmp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3aiaehuep.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3aumsmiwz.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3whgrhffq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ycgbjvkc.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3efnvltdt.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3pqlfojdk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3lgjshrxp.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3vihylrqk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3qhozegka.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3qcljhflh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3xuwghcpb.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3pujdeftm.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3xmtfbfhq.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hokyckgg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3gsdtlsvi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3nbickztz.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3kdmwhqhu.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3tayrxhhn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3cooyrjow.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3vfrynnig.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3oicfdnhm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3jvbpovsk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3axdusbyt.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3qnzdsnih.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3dlhzuivx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3uznhajgk.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3rpilofpb.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3disjftqv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3mixffvsu.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3zxwgqrtl.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ibfukrhv.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3jpwmudud.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3natdfnvh.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3bvrltbac.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3engbnlgx.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3sbsydeoz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3qujnjwvv.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3tzivqefn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3jsquujma.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3bkkyflnu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3yiftuazm.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3sjrljdks.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3btlejhfc.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3hmipjgbb.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3wuaqnjri.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3jsfkwxgw.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3zvtcvrff.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3yqcmsmpf.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3njlbqqtr.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3gfdociwn.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3kccqivcd.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3zoqpinql.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3wrlcufjw.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3rggvxwjc.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3fckarsla.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3vhreywqq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3erqmwdpx.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kxzfaxir.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3hvutpclq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrnyzzdd.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3fldfnpjw.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3qdvbsfeg.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3htzoncfy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cziaupzp.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3pulvgvcn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3uopsnqcr.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3hvixofvx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dvapntfe.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3xukkdnvk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3uvddevwr.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3gymmdyxj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3vikcoplb.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3nmyfzwmi.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3dhtnqznx.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3otmflwel.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3olobtuky.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3goajookv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rnbynywg.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3pqcwsdcx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3wzlxydcj.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3yqxcgkdm.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3wumriral.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3zrvfxjai.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3rzbxorvq.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3mxfdhwta.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdwuidxx.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3rldppqis.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3vyqkhtaq.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3rgbrmohb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3opfqqmnz.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3adnkxpnw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3chkrwjkz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3grtaveqq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ojkwkbpc.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3rbkwuumu.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3jfdosufa.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wywaszzx.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3uxoheyag.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rogewooe.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3nfflkaek.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3fcrnzckf.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3cjnguzuz.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3kmsjnuor.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3hentfgqi.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3chscwujb.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ndjjvswd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3mrdzicox.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3acxxnvxd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3yaghaycy.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3msgevwfe.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfctexnm.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3juqtckuj.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3eluvjdtd.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3rqhsswzg.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3trspgdtu.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3ymlpxwub.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3xsjxpdxs.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3wifuudml.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3bfnjdetq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hsybmxac.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ntjdqmwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lsnotkqm.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fqrjpnyu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mspdrawn.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3juocyrab.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3qsetwfyh.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3dwhblrfv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3zbnwdmeh.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3zjdecfze.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3eepouhqx.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3kezyhbmv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3tjamokre.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3fehelexv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3wjwujuws.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3gvhcswdi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3tunlyyix.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3qbpckdin.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3vmawsjvp.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ewjkqnie.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3jrfyyqow.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3yowkqkic.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3vgqqsvez.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3qozvmujp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3vtllajdy.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3opbslcjp.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rmlzolkp.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3pwkcobma.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3psxqsvvf.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3wsnapzjs.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3xsmsmuds.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3knboxuoc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3tvprliml.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cpoptvuj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dtcaktsr.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3kxsvlhtq.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3oiapwrgc.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bidqpiyf.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3exywyvva.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3vnrgyncp.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3lactwbng.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3epkekago.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3qwrffefn.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3kchstcdh.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ybshqfue.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3jxbevrzc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3aogkiiwy.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3skqgffzg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3tdfxxpbx.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3kvckgnrk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pnmjhubv.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3rxarxwyk.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ztpyvlxi.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3plqbmife.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3cmkjpbiy.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3qosuwlil.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3cpqvqwgr.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fvmxvscb.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3lyxiphhy.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ghmkymwz.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3kffemxpz.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3mqgqtbxc.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3xefzujxg.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3osgtylwy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mnduxyzl.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3zrdukkbn.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3rwohtfkv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3tkqpbwjm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3akgssdmy.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3vapwtvsf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3qwsrllxw.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3lvsefvdd.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kzfjjbrt.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wykrnynz.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3zeorklqp.html


<!-- 参考信息 -->