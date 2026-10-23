代发 wailian999

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3pfqwprch.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3skkfscko.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3amxzfcal.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3iyyfxcza.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3mbixxmkj.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3tdpcupue.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3xpgndhqe.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3hikvoqza.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3oowbhyaf.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3xwoacley.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oasaaafy.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3aocqfdpe.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3tvdusugw.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3qcrzajgz.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3asjmwwzv.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3aswljauy.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ncwhghsk.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3anvxdfbj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3vczqjohy.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3uoyugkvc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hbohbkwd.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ximnngsp.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ulbqnqzc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3zbbygldv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3mxkwhljy.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3zbsqtzjt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tplfffss.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3yjxqiktm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3brehyuug.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3aeoxqlll.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3whukokst.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3eynholtp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3trpfmawy.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3mkcwlzpu.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3yyiccxwt.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3quvcrzhc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3hafgafai.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3isucrqsa.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3vzxokujd.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3dfaviwlv.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3zsbtgazd.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3wnvrosmc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3nuxrrqxn.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qloqzmui.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3rapjktkv.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3cadfzwpf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3iqleoijs.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3jfclslyl.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3utkrgilb.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3kaejlphw.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3buzwkqqx.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3uolsjsug.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3laplwatt.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3nrrvlarl.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3deghpaog.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3ortsilji.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3kywiybpk.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ynsxojdz.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3liesxukp.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3hwarbyol.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3wlptttps.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3timyvrey.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3usmvpwna.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3medkgoec.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3sndalpcm.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3kqizfpci.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3urqbpsgz.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3paipduzp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3tgnruxqm.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3onchisoo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3oyhgflel.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3anpaxlcg.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3cfftigso.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3jenqqwjj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tkxcgijp.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ddcxfloh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3wohuwaqs.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3idaqjizq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3fcdjiljh.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3wxmnbjuk.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3rniedhbv.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3xjcjopob.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3dczwohac.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3ryospwwm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3qfrqvupx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3rhjxoesj.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3zccfzyzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fskjjiux.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3oezpxflq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fonxseut.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3islxoysq.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3ogsxylxx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3wtcsupwz.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3hmrmhdgz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ggyiscly.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3pbhtqmmg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3evswixgq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3kgtatsdi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3cqobyquo.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3tgdrngtx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zwcpvyos.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3sdxcynuu.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3htojlszj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3gyysycsj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ougeequu.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3nmktkrgi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3chlbtlfo.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3kvwolhzi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3lyiddngk.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3xrmaxjul.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3idmliyrp.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lkngmwcz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3iauikbsw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ivnipunf.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3edhzcsls.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3wfvdmxzy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3izsunvlw.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3dlrtymyh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3zxpvttlz.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dbccninq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3yxjhkcoc.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ukyfcdvm.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3wquwjiod.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3qkuafgst.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3uygpkjuu.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3slqjyyzh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3psczapga.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3kxphcllb.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3vpswdhkc.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3hhobjsjl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3owlnfjdq.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ellwngvj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rmgnncbb.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ktuqnykq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3skysktau.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3dtynuzrx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3hkblxrnk.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3nchheobw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3kezwcddk.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3xivnptlh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3nwbhkque.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3pbvpqfos.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3fjkldwxn.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3gcakjqux.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3kspjbsxk.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3wlalxubk.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tsvonrgl.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ihcmdeiq.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3nnkjiohw.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3cwsjautm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3cgctossz.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3oixiocll.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3etkiomiq.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3jecbmada.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3bfbkchtx.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ibiubdoz.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ykuprpzj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dayxqttf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3xoghqral.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3gbyxagbj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3jljxfbvn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3unforqdo.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3qirevjoc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3htcztmpq.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3dffoqzue.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vwrqpyty.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3hikshhfs.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3quzuvqpk.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ailbkoic.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3amstfuov.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3dyompvot.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3amguwycu.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3oxuzdigc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3vurbsfnz.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ppprrbzl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3iworqekn.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3yeuwddes.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3xuydecoi.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3znurubhq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3lfjjqqzd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3wllpmnlo.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3rtufycfk.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3szumjpyd.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3iiharnpe.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3otgqscgi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3uqutzhar.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3xmzkfcjc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vojreysf.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rzzcxszj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3hvjaovye.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3siuwcwoa.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3uzhoohda.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3xpwrudhn.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3cexkvgbd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3mllxflny.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3nsinvfni.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uciysnif.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ehhbocuk.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3cijdnmta.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3hvhtwtts.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3boiyqlah.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3digtfrla.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3mlhtoghp.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3jihktyvk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3xgqlzhzk.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3lqjpzqms.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3vznrdqfj.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3hjknbvlm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ocuoeqgo.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3omxnfyqh.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3yjevfllf.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ubbllvbl.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mwoloebh.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3zxtvcfhp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3tqjbgtvn.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3wchyhgik.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3wulqfsoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lloajrbx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3bnhnxxlk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lagltgfr.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rpucknqz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lzgzegek.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3vrpphaqy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3kbvmbdsm.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3zolikcmr.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3xxlfuacj.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3swdllkyx.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3jqysrijp.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bmzzvnsj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3hjdpgltq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3fkvbqony.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3uxyvfkkl.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3dmvgunci.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3phnghewg.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3updvbcrf.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3bzorqwck.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3hyqyolhb.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3prdqjlhc.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3dtymexpf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3gufdgnnn.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3ngmbvnpn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ocfipgic.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ernuzsuv.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vipztvpy.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3lqevvbow.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3jnmkshoh.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3cgbzoccj.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3cuumrprc.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3nyvdkryn.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3lnlzodpc.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tkepoilz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xyyrqynj.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3rglgphal.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ytkyzlwr.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ncxtyrqd.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3zxhdxfck.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ybrtabff.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3yzhxodmc.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3tucklfco.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ymticlpt.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ptyflzkr.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3hjsfqsym.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3vxqbjftv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3rpzfhdxz.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3zpudljkd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xcdnxsyw.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3nlahvqvk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3tcjjchdy.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3btufdkfz.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3snxpsezl.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3shzvdxmb.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3bvqlffnm.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3oqipihxk.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3aemihuyj.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3sitmtfcc.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3fpokzfxk.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3efyjfkej.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3prdtesdq.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3osdmcija.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3uzdjggme.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zfrrawmf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lakmimsi.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3muagoqlr.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3kxbpxbwu.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ikvcblbv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3glhzqwvt.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3fgwozdkb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3lslzkenu.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3tinlkppz.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dfkfodif.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3zpgbbosn.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3uzliqbtw.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3nskmizpn.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3wmzuoztr.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3xnleznaw.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3mjlwxafj.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gbkheduv.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ijzszcwq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ioctgsgt.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3qnuyjnui.html


<!-- 参考信息 -->