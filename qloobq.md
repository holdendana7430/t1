代发 wailian999

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ohxroohg.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3hzdcyygq.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3wwcjuetq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3uljyvzmr.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3xoyecwcr.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3jwxrumaf.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3goztejbr.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3mzakxlou.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3yvuajqno.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ldbgijhj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3bghlaeip.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3ojizkdxh.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3cuhiohwh.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3jcjiaunx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3fumgowxa.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3rmperttx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kvtwabns.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3zohnxllw.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ozwjnhve.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3dtbglfow.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3qmkbzrty.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3hlmxdyjl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wtqfzjhv.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3fsizpccq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3cbpzipno.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3vxyyfweq.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3eacnksmz.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ehvcbyfw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3mqdwufez.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3xgtbfrtr.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3ayvvrtry.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3jiqrjkyc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3qezosmnc.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3rhbnbral.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3cbfnjxgz.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3bxlupeyh.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3fpsisbvx.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3smfgkfgt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3eaiamjqg.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qanshjay.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3wfcxzkej.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3guyltcsx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3uftbmkpl.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3xiaydgrf.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3uerupsmd.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3tncquxzt.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3uevxzzom.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3sxrkaklw.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3nsdbaxso.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3hzyewqgd.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3coinvxbi.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3arvuefhh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3bqovmpla.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3nxlnibvn.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3xecxugiw.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3kiunokfb.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3czwpwxpf.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ecbpbgrz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3padieujy.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3eupnvrlp.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ftsgenhh.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ziikrzdf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3psjmgplo.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3rzlmcadv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3mhsudxsr.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3buzoavzt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3bnthjlws.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3tcqibcop.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3zfkfddvl.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3mfhgakkz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3smmzzmbz.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3wmygliua.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3rmjsvfwb.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3jrzcpqmk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qnqcgijp.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3achexndf.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3anwlrwfo.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3gayikrjj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3axdrubuc.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3scumfhle.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3pylwbnqj.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3erixeqfg.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3afjmyxqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vfgkyljf.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3hbzzsfdf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uwxsytdg.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vgbpxcux.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ywggxgqk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3bndqqpie.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3dfqoxnwe.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3tkocqgjp.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3anglqwrh.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3ylitybbz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3brrfvufy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3exalsbur.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wfkpmauh.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wksupken.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3trpxhmhs.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3essdwksd.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3nsxtonqt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3trzflvdc.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ylfluxgl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3gmevntup.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3yocdpkgo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3qcshxcym.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3zznyvkej.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3nvcabwpt.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3sqifcgds.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3fyddsgcf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ptugpcqo.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ranqmmxm.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qvqccbro.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3sniwquep.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3dkrgksyf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3ppjpcdwa.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3veorxaiy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3rcfnzalz.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3pgndgmzw.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3zeslflwq.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3xamcmpyk.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ygwvxbmk.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sxiaipfu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3oqeucnxg.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3omtxfnkb.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ovpndjwn.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3avderfyb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3kpuhiwos.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3kjmvvncq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3xwvytbbu.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3nhfcckqx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3hjqxcezi.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3pdtpbxbq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ydipyinz.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3qnipisyi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ozhmzkqp.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3hgpvgvtn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3nakfgbkc.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nevlwtny.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3fgeuvyhz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ijmknzat.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3sajsuojp.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3hqkwzvek.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wtnmgicc.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3asdqpeqm.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3rfoqsvwe.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3fwrmmflh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3lgaqllrw.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3zknwacbc.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3fsgsyxny.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3wumqwzql.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ddpfllub.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3musoexzl.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ghjngcgu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ismhxtxa.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3odqckhxo.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3liubokcd.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3afetmlwa.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3plgxdgix.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3fxejlqur.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3dbtgkmbp.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3nsyygedm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3sqtqhxke.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3nexogkbq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uwppkcqa.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3logkwbvv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3cyhucqhx.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3mmubjgpt.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3vksywcvm.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3xatyauyk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3okpiruoe.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3yxmmkomr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rdoniotv.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3fmrimzml.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3elwlsryk.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3tgmqvldf.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3miaiyxyt.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3dfvxmcuo.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3enhbcwfi.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3kmwedijj.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3mjsnxpcg.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3wjbhujto.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3eaugwcpm.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3kabecpsa.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3hkpxrghb.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3faaxfpqt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbeeujyq.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3khhjtrhu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ymvxipgh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3feeqpybo.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3fsmaaoct.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3sjwchvvx.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3hgcqpgsv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xbmlxwzy.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3pjaxvjsv.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3velrnnuu.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3vyysshhz.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3jsobzgtq.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3twawtyxi.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3zrdyhpof.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3rewumhbb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wtomqulp.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3juvwggtf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3uhtnuvxa.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3hmoumiys.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3qleheflw.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3vlrvkyvf.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3eduxbrnm.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3twwooibd.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zxqvyrjr.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3ygmdbwoo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3jphzygqz.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ftsouuzu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3gqjgphdq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3togaehwh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3hwvmyjcd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dxmjryky.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3puxkrihs.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ygimgezj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3chsnaokg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3wqjqrwsr.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3fmnajliw.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3mtlorzsk.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3fwojkwbk.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3msuzzizx.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qkbvowwg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3unfzycfw.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ezgjysdq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qdclaghk.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3xxqsajmd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ankqtmtr.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3uvcneadh.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3scdpbncr.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3fyfyiflx.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3haqqtjse.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3xtzxyuzp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3rspdzzqf.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3wvxywtvc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3wsmyxivc.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3hoxhdpfo.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3enxrouvu.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3upeyamtb.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3lvskqcog.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3iaapeudd.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jdhasxph.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3gjxhueba.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3leutedor.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3coswvhur.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hxblzirj.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3hjzvsymt.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lahfcnxv.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rkbweiii.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ymslthvx.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3utvgrowh.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3rsxuwhlt.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3gpdryyol.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3kjwdiiuj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nnqoxrdi.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ypkoxurx.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3pkhiuawi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hkzouuye.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3zomkpzob.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3curcorsh.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3okrmtdyo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3equguevc.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3hasrhzwf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3vvsdgesl.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3vxibjqbd.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3zkwyyiii.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3asowlghe.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3djdlvybc.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wbvgmwuz.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3lyokdwwe.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3xrcukndt.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ejjdczuv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3aaefjftt.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3qxoukjzk.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gawjrfcm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3sutooqvv.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3jlftivze.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3yisjvewg.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3gegcoaip.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3mvplrhbv.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3gzlwpeux.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3yktslokh.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3hanewcno.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3sxqdyxjx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3gyjqlahq.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3wqxnrmto.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3fbkafecn.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3xdgkyzhy.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3jpmmbzue.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3uqlvxsix.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3roxpjoni.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3qjeposrg.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3jurfgrvy.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3tzhdvjgd.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pcpzwkaz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3vilpecpf.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3thpmcihz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hotrxkwx.html


<!-- 参考信息 -->