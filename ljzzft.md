代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2byzzkocn.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2jhzbxips.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2hekazplp.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2xqcljlwp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ufmgroeb.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2botqjawl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2uvpkdrxj.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2fcumrvfc.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2hjknvatf.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ubptgytu.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2qewmllbe.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2wrboiggt.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2wrbhblfu.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2tqqgcjjl.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2xrofwyrv.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2xkxsmfum.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2otlcqhny.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2bvzfteps.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ibiphpnw.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2brqujcon.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2otgwulbv.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2izqudjje.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2zrgyujhl.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2xiqmjtyh.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2qmpplcue.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2hkpcmagt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2zrwzgztn.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2xjtuzjzv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2oziaihcu.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2lcrpyblu.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2fvmoymkv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2wuqihokd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2refgxkkz.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2tpiupzpr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mldobqvf.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2rgcwnpku.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2daoudlsd.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2klyebrbx.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2kyzttspk.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2jwqrgaad.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2tbwtipkv.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2waiimsiy.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rvsdppir.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2vxutvdje.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2utxzwzgn.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2eycngvvy.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2nkbsztbn.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2tnvyasut.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2zoxcexfu.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2eoqipwvl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2xomfvcnz.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2tutnxitp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2zngzcxje.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ulrjsqce.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2uovgjbfs.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2uvvjhmrm.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2kdlssjmf.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2kjpczffv.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2xixmicsx.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2nuprzpzv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2ovngoozc.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2hxfyegtz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2unnamlrs.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2woxnpbim.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2tvksppnj.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2pvjkkygo.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2gwpmfrwu.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2zpfhfvpa.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2nqtrnihv.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2iexjsiwh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2qbdgdxlw.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2yeqitqrj.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2zmaxmjuu.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2auicsjay.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2mjuloouh.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2irlidynd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ecloamgh.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2oecxhwhl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2hikzbwyp.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2hpmwinva.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2duilhlpn.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2opjkyaqg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2jsxgveur.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2rtknnvdq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2fivnjdda.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2yxjrepxc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2tkousgxt.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2llxxcglh.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2hcvtjvco.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2bivmuqqv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2evcivrme.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2jjaemygo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2bhaohnvh.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2quofanjt.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2jycjcjub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mpwzexaj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wyfbeuoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cyuuzxkl.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uzypobzw.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ptriopam.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifqrgfha.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2gyuebpyr.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2slkaptwg.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2kvsddpqn.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2zjkroqii.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2lseueiwb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xsppcqnq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jqdgysqq.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2wzkiktgq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2mpcybqti.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2ubuqmbrq.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2velnesdv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2zzsjqppg.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2bikryaaz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2cmzbiqpf.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2rmuqmaco.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2kjczwfzr.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2dlepuiuf.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2iacqeuhk.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nihkrthg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2rfscyiun.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2vufsnnbn.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2evhesbht.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2yohjxveo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ttfdmrwc.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2uiiwvoxi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2vlongiwu.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2fglfvolq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2qepfikix.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2tevgxhef.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2zskedtbi.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2nezftaob.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2artrxojp.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zyuqtyse.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2xdrumcqi.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2tdezturg.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2irmnrfgp.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2cunwieoa.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vtgirwno.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2obvtgnwb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2shcusejr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2prtewpma.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ugoqkzsy.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2dfcfehkj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ndxvfzxh.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ctiylclq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2zngxgcoc.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2znzjavnc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2jatgfytx.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rhhvizit.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2xwjdxhnw.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2cmafpedv.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2dwnonehu.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ydrdhwfb.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2erbdbzqn.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2vdrjpyjw.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qqplvjas.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2iledhnah.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2xfjijajq.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2sjknrwlo.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ifdqjopa.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ljaexbgf.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2dybbekjs.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pmxnfrrx.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ebfjsvko.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fslubeoc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gcnfikvj.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2vowognsc.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2nznzozeq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2uysskuxc.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2egrgnysq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qajtwpcp.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2xuqqieym.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zjzjevia.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2qnryrhit.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ntvnciik.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ohbhgwjo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2aidjgtze.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2igntefmm.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2kugkdktk.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2xgaectcq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2eqbhvktr.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2yaqgwysu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2wafgpzjx.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hklqndfw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2fpqceeuo.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2izckkjmc.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2auqszlhi.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2tqwftivl.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2obttrxjv.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ljddpfph.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2bntoycnr.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2mmccxgxs.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2ehusulpb.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2prvkpysj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2symwpplt.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2xoducdiv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvwbnsns.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mkwrywpd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2magipryq.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vrryhhvl.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2inyhswmf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ihslocif.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2qrjefani.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2inmgfrld.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2vefbnzgp.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2vhatujcm.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2yrgbavzo.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2wkmhusjn.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2vyzmxsvz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2qgwdtbsm.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2niqsaxlb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ccfilovj.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ssntejwh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2fiklwuiz.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2nsrgbjfm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2prhhnotg.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2hhpxlhuq.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2wznxbleb.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2dgkhxgqs.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wvojsvtm.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2xjzavivg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2lupstrzb.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2nzbfnpre.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ingkvrqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mikjcwzq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2bngvcfzh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kneyzttz.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lfcsrjgw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bipqdopl.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2llpifkcx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2hcthopcj.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2wxhjjhgt.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ciczuulk.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2axngekzw.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2eaddvkyu.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rhznvgar.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2pypidbhb.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ppahrigc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zprlkkpc.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kpgdabry.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2cjjejmjj.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2zaoczmey.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ykqilwgd.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2mieciwgs.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2fzlretxj.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2oxflworb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2izaaiubs.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ssswhosa.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2tlvtunyh.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2zplffndy.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2faubyccr.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2rwqsjwwz.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2wdabnbqb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2uysysbbe.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qcbrpwyg.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2uozdlkfr.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2lrzybgja.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2spwvjjhq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jzgujfjx.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2sujbvhdg.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ofxmvdde.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lrfptgcg.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2yohnajtv.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2uqqdzjze.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2rcmbgtrp.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2soahvgoo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2cnicpyhu.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fruyebwt.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2oynhzoxl.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2djhezkci.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2inrxadzv.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jpcfhxey.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2vmtjvfut.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2zbmoozqp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gwcddypq.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2jfmebuzq.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2mjyfoknn.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2uqjmezag.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2gscxuduf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2skejfzez.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2foeisfqc.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pvaigbwg.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2hypbdvju.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2meivwhvb.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2dbynimst.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2jbnloyss.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2xhxiremw.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rpsrnolm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cdwrznpf.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2zydwovzw.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2klgeoucb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2uzhkbwui.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2gwkzaqlq.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2gnucrrfd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2buxewzlo.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2rtyicqby.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ybzbcxxq.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rcdkjvmb.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2mgxwklzm.html


<!-- 参考信息 -->