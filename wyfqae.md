代发 wailian999

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2utjcblao.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2ewrjzafc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2aktfhxvn.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2nebkefql.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ejdbeant.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2scfgdytt.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2qrvpclet.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2nolsldmg.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2lsylgqey.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2iiaetxii.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2bzymnqzq.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2gvvguqzd.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2aeztzyvy.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2swducprr.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ooflcnit.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2vhdekhfi.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2tlvazvtb.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2bjhcodyb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2hlsjkish.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ecxjtzyv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rpydabkp.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2glkigiov.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lfjypwny.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2kewmmtix.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2aonebhjn.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2wgcmwiqq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ntfbfxho.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2sklcdmdb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2kyrmkjtc.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2gkxhitye.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tuhtgotz.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2pcwsqvwi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2svkadzgi.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2fffhiakm.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2atpnxeuk.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2wfucfgno.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2vjwkvsph.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2szdwwofz.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2xrabvncf.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ujkvxmbo.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2hyeygasm.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2yqykfrzb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2codenzwl.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2sxvhqcjb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2sihbryrs.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2edvwcfdm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ssgraebr.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2tmwdinec.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2zadscmdw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2bbeftvjm.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2poordjyq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2tyxwivuh.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2wsiquxuh.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2sxgjijke.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2nwkxtyei.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2toqpbtfx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ejrbhuzk.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2zraqupez.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2jfquyzwp.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2lqtcbqfd.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2sgzjorwh.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2zuvahjyp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2rbhmztpp.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2fwdyfqug.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2hpkkcqig.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2lyjjgeqy.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2nxcpattf.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hmcomnil.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2xxisbhls.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2bnygncvf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2uargxxxw.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ovdeqstx.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2pelpjcia.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2izbfjokn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cifqhzun.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2ievckqjo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2jasipavm.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2umbymmip.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2xfkiyqrz.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2bweufvwq.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2rscxbnex.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ltccluby.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2grymzfgg.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2shtjjfzv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2jpjxkvbn.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2vfcvemgx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2lafgsuiu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ytpkuael.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2iilbpsau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2refwrkqs.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hxeutcuh.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2giawrfjx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ggzrazgv.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ptdexulo.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2cyubtxrc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2glcwaznc.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2aukxkjkm.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ldwgprro.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2iucqhnko.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2iezurhqt.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2zkwrqyub.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rmlotafx.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2rdtdagzi.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2ikucboio.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2dwstmusg.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2xuqjljmy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2nzmfrbhd.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2mwneugjh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2wndlmjnj.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2mktyrsce.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2mthmsnpq.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2glivkbgi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2xsdtabkb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hwwuoadp.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2wihhqwwy.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2zwuxxodi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2vloeageo.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2rwaxxavo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2xxwyjjrm.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ogfwqogi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2lbufttdc.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rsyqybvh.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2zijfovgw.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2rlkqbypz.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2jhqifnzn.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ydgxbqbl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2btkqxtdb.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ctlamjxv.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2pnnkbxja.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2kqmxqanl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2stqrpkwm.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2iufaoppj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2cugmxfgb.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2hhyhdgsf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2rhcxmqzs.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2zdquvcwn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2adtsagyg.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2yauqxvwz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2lnazblle.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2jpqteqos.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2idfkigmp.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hjurmgel.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2azacgoab.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ehoangnp.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2wwxuktlb.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2zunjsbpw.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xubwclmn.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ejupogpd.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2acdkfpod.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2kbvtxjqe.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2gswoclqn.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ejitlwpa.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2fcslcyjw.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2zsvwhufa.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ctdnzvuu.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jmxahaku.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2gymcjdio.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssgetmjn.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ixiwjtki.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2zaniwuhu.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2cmzliipc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2qxyzwtrm.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2daszggsi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylguewjd.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2hfddjqcn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rsreluiu.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2rzsayskm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nzgcryta.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2fscmuahi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ygenyrqs.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2asyaoail.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2bpghqofr.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2lyqxvtsc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2mahtoqbw.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2gkfqxtck.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wmusyhrs.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wjlrckpp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2rtauybhn.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ywtjvazi.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ouaqrbia.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2plcgkblp.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2bomtoksb.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2uoskijta.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2oojccvxg.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2unecvfpz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2hmkjlmjo.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ykulvqwi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2emotzckr.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wpcefqoc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2siaruplp.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qrdrvhsd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2rzsmdhfk.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2vuzkjhhj.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2rchamrir.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2pdiouytk.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2gmreihmh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2iaegjicr.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2dxxuzxsg.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2hevrkhln.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2exqtzbyu.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfagsbzh.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2lehdqwwn.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ccrfxbsg.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2fdiamcmc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rguuvbrh.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2aktuynpl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2honglvln.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2wjqcywly.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2uxdiiwlu.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2qtlqecmt.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2slqsyfte.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2vadvjwqv.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ahahjlru.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2dubjkluk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ghvudmuc.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2xyhltehn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2fqmuptja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2amszcvgz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2uwwmgozk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2arbssgpx.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jbxvtktt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2frectsca.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2hhriioal.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2badewast.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2flqolpge.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2kejhddbc.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2bgjkqnyy.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ydnmnfoq.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2oyzckvyn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2pzsxmxyq.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2dgpyulvd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lpxybhbq.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ezmkqzah.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2yghvhqja.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2phdvseuv.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2jjhgaskw.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2uniptwij.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2dgepocwi.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2adtzdphd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2pgnknwuo.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2dunvziii.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2jiymocja.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2vythsegp.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gdlkjqkq.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2jkeqfppy.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zkkltjmi.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ycphkggw.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2heswglmr.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2itjpgsrg.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2gzizslvb.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cpjqqkeb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xfbcuiam.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2rxjlewfb.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2nirxijoc.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dnwmtzyx.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2kfhulmil.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2ngcbicvb.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2dzphayya.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2gogsjgvv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2ykqhlqqi.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2gocrexln.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2kraylqhr.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2kbgrtlac.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wtyzpfxz.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ghvcfjou.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qwkumcvo.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2uweiuxvk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kpvfaicn.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2uergqixo.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ejkbgexm.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ejigrdhc.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2vomqbnkx.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2smmvxoou.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ccotyjch.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ouugoetz.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2uejtgsvd.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2jmiedmva.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2wqbjghpf.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2wbhbuxnx.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2flstzjwr.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sgvmemrk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tmkjufod.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2vhycwmig.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2graqoymx.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2bfwmmqyg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2bsztwssd.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2wrwgzhae.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2ckfhdqva.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2hpahuxih.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2gywevrvm.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vhcjvvtn.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ecrtoxgo.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2yckflcrf.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2dcbnqoqp.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ytfzrowk.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2udyhtwwn.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2uhpshzug.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2lgpdessy.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2pvrjfugh.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ajtxdcnc.html


<!-- 参考信息 -->