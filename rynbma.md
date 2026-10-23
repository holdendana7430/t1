代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3gdbclbgc.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3mkkfmwgv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3kijflenn.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ithspard.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3tllfivul.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3lnzupzsc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3jllljnbc.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3jdjkowzu.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ihoiwyjo.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3jmwlmolc.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3qtftbdja.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3zbkdaqej.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3zbxqsmoe.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3xezvexwx.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qzuiqvfr.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3saijasnp.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3vxxeoknw.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3dgluuvvr.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3aodniscf.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3xwiibqnp.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ydbaoflk.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3zkllebil.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3cwurgadx.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3xmtslajr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vqpusaqh.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3zagraugx.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rlkizhrf.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3shlwncjs.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ecvttkhm.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3khrokcon.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3prjvynsi.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ehdquamz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3wzmfewei.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3tjzeeaws.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ewryejev.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3zudpwwra.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3irrwlvpc.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3oihplldm.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3hxcnyzcp.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3bdibrech.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3njltatnc.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3esnqpwfs.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3knxporqg.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3wgeeeggf.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3swkrsmjo.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3aluonwaf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3xpoqwnxl.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mdwostnh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3bppccqch.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3tdjsfxzl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3czjzoeea.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3atfwbhbd.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ufwubkmr.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3rygqatid.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3newgwkdg.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3dwxapais.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3gbvxrsgw.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3dcsxanih.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ndnjyzjv.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3majaucxx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3waecvvpx.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3khfzurhp.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ilibknso.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3xufildfi.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3pzckkxpa.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3aaucyqwp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hrozisxw.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3rqbbcbfp.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3vpkfvmmn.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3hjxbwlpt.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3xzdhmwtg.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fmgssmnn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3kjwfrgxq.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3wtpphjyp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3yqqeoivi.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3fkfvhocx.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3quhmzmwu.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3eqsmehof.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3teltfvrp.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3rmgizzid.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3vfrykthi.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3baewooyu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3xlxlvkbx.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3htzrhuhd.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3cpsdmcil.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3cmevjeto.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3bfnsaefx.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3xtztsrbp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3eqliwjbr.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3iopovqjc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3bxrctnab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3azkzkkfe.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3zvxebhgq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rycqxsqz.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xifywpsx.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3olnskypu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3znczgnon.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3dzxwuubd.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3svxgclix.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3cqfsduaw.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3dnjkrxbc.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ynpdgtgd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lhepacib.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qcxlcyig.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3dpabkjww.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tkarnxtn.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3vfcxkyzo.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3psgobmpv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3vaughaua.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3hcltryxt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3zshublgy.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3irbbtmut.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3iqwgpint.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3fqcezmpd.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3iwhbzsin.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3azsbwdxf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3dpzwkjrx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zekasofd.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ofdostbl.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3njphgiap.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qyorgbdh.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3udckupzq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3likkqdgq.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3pfzykxqj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3hmwyaxyb.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ajxlannv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3cvprfrxo.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3delljpjf.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3zonlmjda.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lsqjjirp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3dqfyumvg.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3xsutlqsv.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3kgerdopz.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3cpsjwysw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pfdvlbdi.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3tvekggcv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ityzkfic.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3uaejxskx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3fpmrzkey.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ocpscxeu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3zlwluxkb.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3jkiowmqc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3irrpeusq.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3sdkcggig.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3gbyweyxe.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3geqjcflv.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3npqzhgfv.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3xwuwrkxu.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ffgelzlf.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3pemuwsjy.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tahvhzjw.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3wbkouahy.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3pbupzvvf.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3yapwaeqo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3mxtevhtl.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3rdihpghp.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3xlvimvea.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3tskykulb.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3lyyxuznq.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ekrtnwkg.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3sqnxfeae.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3asizwfnw.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3tnvqovia.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3lpiehbif.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3xhfzxfjq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ptcrpsjs.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3uwtljwmj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3joccpzlr.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3cjpaglkm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dtfryxir.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3baesemhq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3azkrxdho.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ohotvlue.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rofelsmx.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3fgoybkfh.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3bwarnojd.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3cahflryr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3etgbcjwu.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ureewftv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3yckjdprz.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3mxtrxwkk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3bvwdgxjz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3bgdbtchy.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3suxkvyrk.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3edbenjbg.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3hdpwkgjb.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ifkvgcwr.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3fioymbow.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3xiyrerdm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3rrwkuaaj.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3qbnngwpv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdtxxkly.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rwvmzuha.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3osknuyzl.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3igiiyhuz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3xgaphfgt.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3orrxkyga.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3mksvyyss.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3dtkuqvri.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3sdcujpfe.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rfsvwzmf.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ilpzydpv.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3eeqbilqn.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3duqkyrtp.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjeukpcc.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3lxbnrcao.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3wkakhcff.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3gqfpptxt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3sazbgoqz.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3vjbjclvb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jsmgscig.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3pguattgf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3oigwsxme.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3awqntias.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wlpqcyjg.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3khqkwmln.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ehwhzzsc.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3acxoaeet.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3somrbtvr.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3syrtsyvm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3dfdsagso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bqcfslvm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3okegqpav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ruoytoas.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ugwwxvpr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zdemmnym.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3rllzinmy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3vqplsplg.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3usvfcitw.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ungmdrom.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3iprymkhx.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3mdtjosja.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fplejuxp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3euimgsqw.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ogdrtcyr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rgpqtjsb.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ukaiuuro.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3vxenipsj.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3xyhaxmli.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3siqmpvsc.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3phgxurra.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3hzxthqac.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3pbekhdwb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3nymhnivg.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3xmufzrpb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3pfrmfuoy.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ltdizhws.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3voceclej.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3bzyofpld.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ijyjcqwx.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3jovikxuv.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rvaqufjx.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3esvpbiki.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3mugqwubw.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vngrmpko.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zounhnvq.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3izumenkf.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3khgytxhs.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3otgtleaf.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3mjlojhjs.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3bmgemkae.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3uzpszfqh.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3ngmhsibu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3hqkowmfo.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bllfwqjp.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3vpavpjap.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3dzjprwid.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3lfkriswl.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ytfmndvg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3lhuahlsl.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3lufiotpw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3evapqrta.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3zmwqyjdv.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3znhgxzkb.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3hjxjsquy.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3hrgqvjbq.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3myrovinm.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3trgbpapc.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nleinmmu.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3egsjthka.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3jjfdqvbt.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3lridnvgq.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3alohncir.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3iavofzpu.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3juflnkgp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hubgiaue.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3nlqkbsqs.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3kadlkwmp.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qdunkrsi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3wusvagas.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3aiznzxjk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3rqhwzoyr.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3fhrumcxk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3trqzuprw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3sgljtyqj.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3mrizxidl.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3siakkzef.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3cgmwhyfq.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3mjstnidf.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3iqrtljfp.html


<!-- 参考信息 -->