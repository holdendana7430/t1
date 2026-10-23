代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3qxchowrm.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3twpactuh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3gjkaoluw.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3jvoyvpew.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3chlamesx.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3fomdfrwx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3iwiuslps.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3vcuuimla.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3nyjxqfvw.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3cvteqmrv.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3kpaamrwp.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3kbnvpjrg.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3udigjqvx.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ifjbxtqz.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3dythxowu.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3gqdwdpjz.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ivfladnm.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ibcdtqvi.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cxupmkuv.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3zdztxwny.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ebfhtdmq.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3fluxpqcm.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3xlpgdjlm.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3gusyzxam.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3vdjwpqqs.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3utsrlamj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3uovyqaiz.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3zquomqii.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lvqvlzrr.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3lqvjsujo.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hazffxjb.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3igpwqydw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3wwokasgk.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3tzgucdcq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hicrkdax.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3uzwoghrx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3dgcbaxdt.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3takkvbwz.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3jysaqgdv.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ylioaquo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3ohlbbvnh.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3xdddyxlh.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eqdcursi.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3rtjjyadn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3zwlfjepl.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3zapcxoyh.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3qsbondwm.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ftfszelz.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3wuzwpnum.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3thpwikhk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3qzhzkjll.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3iojaolqd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3jipbnsvc.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3zqvapvqn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3exwnqxox.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ahabbhsa.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3weamkepi.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ckpigomf.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3oijcgytx.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3yfmthzll.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3nejnnrnz.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3gihnymvq.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3zcthpvia.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3edvkvwwi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3tjxvmlsn.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3yohmquwy.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3wconjcqw.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3tzypciqe.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3eqiygqfh.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3zpcwrpyj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3colwhtfm.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3uicfdzsc.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3cxhpfdhe.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ifaqxibg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3odulkrde.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xzrinatr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3acjoaixp.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3taoktheb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3zdlvegsg.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3anxleaar.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3xidiawyv.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3chmljafb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3nhupuhjp.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ndecstld.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3vdgkddzr.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3hwntlpbw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3bkfmlwey.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ufcxjprp.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3omyvepvf.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3jauruoos.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3oofgzljz.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3tdaigyld.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3awvnbjrp.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3eiytixqf.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3yfktbohx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fvtoxfum.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3pkzfiznl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hutjjjss.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hyyqbkmw.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3lkrwpezy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3binqaxbv.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3nlvggwuo.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3xovpbhlp.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3lnitvupt.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3nnawivlp.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3bhnzomvs.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3airowclz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3gkorqhbl.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3qnzjvchs.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3dtlilltj.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ytqvgukj.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3pgflicdi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3zatqohqs.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3lrlfnwqb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3jjwazdvy.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3xricggeb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3cibwrtma.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3itfagswm.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3qxmysmpe.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3licyjkve.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3vrtieuhh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3xzidnglp.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3udgqgruq.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3nskkziqz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3pzfiaoeh.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3yxxmroys.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3gcsyiyyz.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3dznfejnd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3bjyqgyuz.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ybwdzurt.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3osiwkxmu.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ttfkcbot.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3fzoxtaeh.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3yuyozgfj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3dcwxwvdr.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3aqkyzkam.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3bfvgttmx.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3zqhgnqgc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3eijwjitw.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3hddlfcxk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3eyzkpchz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3pimpocuo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3esfjrans.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3wdoyfqzt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3oenfjqjr.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3eosdzifc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3uzaucnat.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3hbmvuvmz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3hzrziwyr.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vvhfkmzo.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3djsijybw.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ggdhwnyl.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3dothhqnl.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3hszhxxbk.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wemqcawv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3bfugthuj.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ncnlsmxv.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3zphicxoa.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3oxjtsoto.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3qliswkas.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3yerflumj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3oxprxbxz.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3zykoxtej.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gfvuimic.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3irivrrtk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3lqpmmdlo.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ykkshnzt.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3kgbornna.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3huulhedp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3tuvenmdn.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3uaswnskq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3quqcayjm.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3mhkrqtcf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jsuurrax.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3bvdbcjxi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ffwvqgtm.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3vdtfpbxg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zhphvske.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3npqnlhxd.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3gzzawrrn.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3qllyoobm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3aktbzeqk.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3buhzmgqz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mcdfwuey.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ggcvmpui.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3atqugsqm.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3abxrqqpe.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3wwkqkblj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3fmnoiqva.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3xnwxolff.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3xbyjcfkm.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhvawwaz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3zshavzxj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3vnucgqjb.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3dvnoosoq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3oxxmdoud.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kcwjmzka.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3wqbdqqjl.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3woidifax.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ojmxmcwz.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dapsbgpn.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3wxflefoq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3menzrpki.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3uysukbta.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zybijeow.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3yceztlds.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3rehlgdgg.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3rsrtviaj.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3knsiawne.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3gbgchptr.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3lunidenk.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3qebstdtv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3plbusqjy.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3qxfnnkpp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3goniabrm.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3lnbjpzze.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ndosnque.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3rllbghgp.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xwjtjrog.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3yuyywonc.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3mrphhmbv.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3btiqmpvu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ouzuyfoh.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3uobenzsv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3torynsyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zhyhkioj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3pehfmiyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mvcywrnc.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3izidlpgt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3sdspegrx.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3utovznaj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3mklvdzmt.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3zllwitli.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3dsmrtjon.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3fpbhscru.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3rvejwrek.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3gubmsmqk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3jrhsndfk.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3uszixgdg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3flasopst.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3plhqdmie.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3saapmusp.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3crskbgkc.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3cpzqqqqw.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3svgytjve.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3yrdrrmtl.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qcvcbftp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3uxzvunqa.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3fzdskctm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3jbojiwdn.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3wbadyjej.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dzvcphyr.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3xbpqfnkh.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3yxdzgqfj.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3nyprkxpd.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bduibndr.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3okyvqeyk.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3gfdmugpz.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rvgsvzvn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ihftkuua.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3qldvfplh.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ucuoyrrp.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3utbczcax.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ogwqkizt.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3yjtuavkq.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3kosfzpac.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3nniglouw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ttpmuyhy.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ybqbncqn.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3gedfzoqq.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3rgihtvmv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3jbnjhncd.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3nadogkpy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3isdstlkp.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3aixazrvj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jkimgudf.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3zlqmnchh.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3vlqmelvz.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3xckpjukx.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3keoqxftg.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3aetnyoex.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3iobxmqnf.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3pyeremna.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3vyyuodxt.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3vewjlxlm.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3fquglrto.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3hnfweikp.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3fvazrlju.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3khvzpbzt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ozuyyjbv.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3yknaeupq.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3cgopebsb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3iarngvpu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3yvsjefry.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3wuetfcvh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3gxtsbwnl.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3foywrsrt.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wyztvdya.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3drdoxmbj.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3zxahlbbn.html


<!-- 参考信息 -->