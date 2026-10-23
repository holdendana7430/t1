代发 wailian999

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3wfduxctf.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3nystovku.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3mjdbvwar.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3sgtpzqoo.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3bnhofesr.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3hgbhfcjh.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3joeqyfwq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3qrhvoqqh.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3lafkbrcy.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ccnwucao.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3xqjkljcc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3prsmtftx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mrpauarn.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ruatcicv.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vwewdblg.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3dlzrmgxo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3ocjqmwci.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ydvbenpc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lctbvdsv.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ueodptue.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3mmxczzlc.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3cwgbsjnp.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3qahsaxsq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3jthdtpie.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ogwkbwva.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3vlcnwjnt.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3drlqitzl.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3vahnfaiu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3oqfulovu.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3xbryuywy.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3kgtkellx.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3jtzewrlw.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3qkuumsht.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3moyatgug.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3vxcsthdw.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dewjxfpm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3nkssfcmv.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qbvctqjh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3iqctpyjt.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3vqapurhk.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3bhnaajtt.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3ypteizgj.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3pcckmwew.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3rxqpivbv.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3fncepqfz.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3bsqvvcni.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3lznrjqbl.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3wdlotxjw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3nokvyuzn.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3kssfxmxf.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3xoceiqhr.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3xpjwzpix.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3qhlgtyfr.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ujyqnleq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3olqsgysz.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3wbyuyesu.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ywpmuckd.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3xcbsmhan.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3cthjvmtr.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3opvbjmbs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3idjsvrti.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3rtfbummd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3wythbbyn.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3jlaopexh.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3zkihmxge.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3pamhjndr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3llrpcoxj.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vmfftwfl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3jcfowwin.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3huhzpylz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3zzwvqarv.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3dhlduwec.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ownkpvme.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3irhtcxxo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3cgclerhp.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3nugdwphh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3arjpiers.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3rezbvchh.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3lyyrebjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jnrianmt.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ozebqsij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aembdwvo.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3veuolkhu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3zhxspsiw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3nttwjwrh.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3fpqkkxng.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3dlmkonmy.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3iojgselo.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3akikpuak.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3rpuevzaj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3yzpbnqhj.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3btdmbhvd.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3zqnmvbrh.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3lwapyxeo.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3njjbbwcc.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ztexexhk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3iunzwwji.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3tfxoglcp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3jabmyvnl.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3zyzpjnlu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3fioimcfs.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3buvbrrpk.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3chkdacew.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hiiivcfn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3gsjgdqgu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3erifblcn.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qcnieaqe.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3fcglwwlv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3vlkremrx.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3qnhnxygh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3irzyptld.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3haudeamr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3jlswiiqc.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3zpsyualp.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3sonmonbr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3eawsnwqa.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ewykrxai.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yqbvgiue.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3mcbpynwu.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ldwrtyfa.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ovuxwdef.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3vulfcpmp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3avlyhwdi.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ykzmzjfa.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gpnfprct.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3mfintwqk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3eyhogvar.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3bqtfugfo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3fuggxznh.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3pgieriye.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ohgcddgb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3jqtxjxmp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3iwmkvebn.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3gtasyjmm.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3hngwdaep.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3qwwkqjiv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3vicmwers.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3fhodlhnk.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rkpzulsm.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3pqfawhes.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3qzzygtfc.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3keybfulq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3halmqkln.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3jfujmtbd.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ttytxzjp.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3kfbuswwn.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3qtzclgwn.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zukgjjpg.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3nllxlijf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3cdayqbbv.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3mhueunxq.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3vzwtftog.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3khjbeuyd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dlyxcepr.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3mytkygxn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3bbvaqdlf.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3zpcjkslq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pagjwqdw.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3gkntnpfk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tlzwtjru.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3vkjauoqf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wbkwxkus.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3tnlbkeuv.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3yyklknhz.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3elwqzanz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3miksdeao.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3xczgqraj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3jiewxhdp.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3abuzjxiz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3dtwfzngy.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3msxvdgfy.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3vtvcicff.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3zizzclpm.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3nzdqvnts.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3vygtctax.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3iqyzdwcd.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3rruscacs.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ygtprouh.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3sksbjjfl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3xcnlewca.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ipzwguip.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3wyztsped.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nqipvwbv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3bfixadkf.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zcqobqmi.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3fnabnjwr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3jejtnjkm.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3nhgpxrpj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3iysjggpv.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3gcophzxv.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3rdvnoxlk.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3fyceyexb.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3pvojqbds.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3kzmupshi.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3uaoeprkv.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ulwjdhdv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vzevpvwd.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3oioxjirc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3umgilkud.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3vykvgwzn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3adrwatpi.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3cmbkzlqa.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3fpkfsnft.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3npulcmqw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3smdvabuv.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3dmxetcuh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3pqotklbg.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3qmhgixob.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3nynqnlpn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3foshldru.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ltdngawo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qmmwnejl.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3juiaiajd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3oujfspll.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3cnouxdwh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3qryyrvus.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3jcxhvckr.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3bhzcoolw.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3plbqtiqa.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3exgyxbds.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3lgkarczd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3fvomeutg.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ovglnacy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3glwiribk.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3hwnehehf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ttddehil.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3blpqbqpe.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3dyyhbsbc.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3bwgfohga.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3vupxxaxt.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3yutrijya.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3bwuwmutu.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3ayydbalf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ogsianku.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ztyvmzii.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tighavec.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3cnvtnenu.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rejmfvjp.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3uvvzkvly.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3hmczzrfx.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3zsxxltis.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ncunomkw.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ogmrtvpv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gdidclwv.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3imzirwcn.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3pkyvcxgp.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mangohae.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3itksufgf.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3xvgvurhm.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3yanqdabw.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3epxenirc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3biqepwpg.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ulsmvyum.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3krgxuhag.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3bekganzr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3prfwvvim.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3obbrbofl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3cmseukby.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3mwixxsbv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3raoiaoce.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ygzizgyf.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3ytetwail.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3zvnquzau.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3nbpdfopj.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3tyzqyyhb.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ugvrfrbq.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3nbmpmriu.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3dayzjifp.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3dzqvhvpk.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3khscipur.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3bjksafvp.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3cnzzmrrp.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dtvbqsqx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hnvlidmz.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ajhooryf.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3evcovxlo.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3vwnwqyre.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ijdcyzrz.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3zhbrvrrv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3xzrjziob.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3ebrckmuq.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3ewmqoaum.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3iwfambzh.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3zpabybkw.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3lmeexkvz.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3xxwaleck.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3ddenddih.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3cxpcnhok.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nboavvyp.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3iqtsoyqx.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3dbnnrumo.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3sxnxqqqn.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jefnfzyi.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ycvzjobt.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3efjlzpdh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pnaqjbjw.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bnzcntob.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3hzfypexe.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3rhfqlmax.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3yyiahzrh.html


<!-- 参考信息 -->