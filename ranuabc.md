代发 wailian999

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gbohhoczf.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcllchze.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzjpynij.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gpctfamnn.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/ggdbshata.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gannaczot.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ggbzomkap.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdogavpi.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gwfouzwzw.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gvsmbvrnc.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkljcznm.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gzqwdsotw.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkotedlgz.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gdvkfcoqf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgfjnkep.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gdggwahha.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gfvzwyjyk.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqlxwatx.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gfihfvbbf.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gthyglqxg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gzyuhkpbz.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/guclpsfsy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gmkhwpgvx.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvklbyhpv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/glyzvwadc.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gckizcxbj.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuepfwjt.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/grasyftzt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjbegepq.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyvbhrww.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gxhzazygy.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkwflptv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkibgnmva.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzlplzke.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gbweangot.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gzevfqdbe.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbwanlvz.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebqquxzu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gbiteanyb.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfyussmb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqahpwpb.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/giheuysib.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gontfxrzd.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gorxfvsih.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdsoycay.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gejqacxue.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojkhbfkb.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvqpzpzm.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gccxminjy.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/giqmezkfg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gufjflaru.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gobpjbhtl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyinpxdn.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/grkugiyed.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gwelhbpnd.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqnrydca.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/giubbbcua.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gakaffjsk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gqetrgzbx.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezhjlxxf.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gygpkawfo.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonhnxsfr.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gclmhzhft.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gvpylqtbr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxanbrjs.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbhyooay.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpsctcvf.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwpnocop.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueelyexp.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gmhcqcvgc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabhdziwz.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxqvsbjl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/ghrwubhji.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gylzqgtun.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlrzvmze.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gsngyeyin.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gudwktbsx.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gpfkwcpcq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/ggbkpeoci.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giknnwiqt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/geczxlkym.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxhmcydy.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gsnvddgxb.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwajefeda.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgpcakhl.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvtuojig.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gseaazxtb.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/giepkpupl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkhqjhty.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gfvdrzjtk.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gizrohwte.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmeeplbd.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gywyunidv.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gubpydcdt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjikksqv.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gronktjqa.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/guwlklhia.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gdnlggixh.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqquwzfw.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyubbposj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnzkhoxu.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gfbogifuy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuhmuecx.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gnlatckxc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsywysso.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gntabxjtz.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtptsblsm.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbaqbgozp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/grsptzrnx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghluawwrv.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gqbyagkmn.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gpeohaqkw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gpwvmudov.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gdteakhlp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gohxnfkxp.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gauvtnvyv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/geascmhpi.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gypfqwjba.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gphjkogfz.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrfootru.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gzmovyqys.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbefqoaba.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/ghbjujvkk.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnqmhzok.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gagjndfzv.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/glqinbjqr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaarjoauo.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdyroekc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/glujbexct.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gvykfgcym.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxsacknh.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gyqxvevcr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gndrniige.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrpsdmni.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/grtqotbeq.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgipkjrg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/ghlsjcghu.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/goatfnqsv.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjldylhvj.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggeoiqtka.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gwxzqdghd.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/glctstdqf.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gcrnjnrhh.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gttgmxfok.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxhzquqp.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gbumqlvus.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gfttcpfhh.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gbbpnruxe.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/grwvobduq.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gmtastmiy.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgkprcyh.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gltfnsqvj.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/geaxrlgqu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjxjbhriv.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvjciutn.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gafuzfcwb.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmmonooh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gppshwepw.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gosvwusny.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzbjtssrb.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/grkghebil.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajiuhtis.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqktanml.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/giyhooaex.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gcksbtnug.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gczimahnj.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gwkulndnn.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gmkjqodos.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gtgwkoivu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnasheskp.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gjacwdoxl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmocnvekw.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gymsbvhbp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gyowhwwsv.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbarjusbh.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuvrkncz.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gelvemrnn.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gymvtwebz.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gqkgsprwb.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/goixipfbp.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gviwzudvz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/glqskpwyx.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywlmwttq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkmxvsetq.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gmwshjjad.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmjaaiktv.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/glyojidvo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gqoqinkxm.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtmxyvry.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gnziodgec.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/glonwvcbt.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/glzxehgka.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdogmoazn.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhbgcoeh.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gaxjwlaqa.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gyutqztic.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdnorgdky.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsdwzedv.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gakegairu.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/gveuycmtc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gknrgqqec.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/giqcrrszd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/ghuypdspl.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzumafhs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtakzzlgf.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gtrziotqp.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gotbbczuc.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/glyqbahqo.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxsyaoku.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gamqexkng.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gfzfnopgy.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gyqypiuna.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfsvuslx.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghtbakbbc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmylzlhxt.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkprgtof.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gpaezqtdw.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gczaxqwrb.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayvnxtoq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gsctkhglh.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/geljpawct.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbhluwev.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gryggqrem.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gqstbtpni.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gbejtxrqi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasixzplt.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gmelseedn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/guwljkvii.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gzbomqoks.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeegifnd.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/guxxeydqn.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gdnwcfgoh.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahqzazdr.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gyrvalleq.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbpztmle.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwglzmgl.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvfychql.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvutwoyzi.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gaatmyuwk.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gztnwdgkb.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkwbctat.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gleqfztpo.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gynixcedh.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrxfjffs.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpadqzgs.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gnfarrrdt.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrpyzoam.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcrnlxjn.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gkcsgkasu.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gddlindaf.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gquqmkfjc.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gissghkzt.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhuxumni.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmervtwqi.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbzkulvm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozguhjna.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gtcpyucdq.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjnbazac.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gntezfvtv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gtffgyytx.sHtML

[T23] Swift：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbhbsezx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gazlwabgr.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gvocqoxeq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzfzdrip.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gtqznqpkl.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/geofltirn.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmieirttw.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuuynacb.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gmizkzumx.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gvsgwdjmt.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gtzujkkwt.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gpmuukhsi.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/gjxxwuxay.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gaiyoxxgt.sHtML

[T30] Swift：协议
来源：http://baike.fanxiaobao.xyz/Article/details/gcbxkuana.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrbbzzld.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gduvheozt.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gujepjqpx.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gtruaupxy.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gkhitfrxt.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/glfybgewh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmrhhkef.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gqmdinsmd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/gekiiedes.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/gopvtbijs.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gbywikatt.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghumaosqq.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gviobfdrf.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/ghbiodpaq.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxecrksi.sHtML

[T38] Lua：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giboqgfue.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayxulsuz.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmigdkfu.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gioaiyoja.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/gsiqaamua.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fanxiaobao.xyz/Article/details/gjijnflvy.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmontuqu.sHtML

print "Hello\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/giwugiauj.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzzwsurm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/grvitsmrf.sHtML


<!-- 参考信息 -->