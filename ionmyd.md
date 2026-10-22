代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2sdkfarfv.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2ljyymiff.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2youvlvxu.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2musuemni.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2zydsjsqi.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2tmpradqv.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2gvomuzpi.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ncfstfqg.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2fduzhowy.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2dvnjgiyg.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2htkagkuj.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ubgoiocq.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2qqmzjmnm.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2mbbuqzsa.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ialipcgg.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2jiukyvqz.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2cznllngi.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ejrovill.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2bwbpwhmz.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2cpkaxiiy.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2sbevsdfe.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2jespdcsh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2jjvxoshy.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2hozuwfxj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2buuackcd.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2bagqmcmo.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ezfxkbcu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2wjhgzzpc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2zapyrryj.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2bdkkqtwt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bxzybraf.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ramvpchg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2mlnfsiil.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2brsmsurj.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zgfvzhia.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2nirtbshe.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2wmnmkdel.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2fjwmgyiv.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2krsxawdu.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2uskafqfc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2mtutaikl.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2fysnuduv.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2joxonpsb.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2azqhmeow.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2bryostrg.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2bvjdulpe.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2tokrapru.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2bjrvcpyt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2odizwdey.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2geojjkqa.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2anzvqygj.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2fzhqhfrt.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2xzhbaruo.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2krfqrdix.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2rwjfwhco.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2jvdqpaph.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2zblovvcx.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2wanwxeue.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2efayoycy.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ilqspdql.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ytnqqnpn.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2lheflude.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2exvjwaht.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2rwiibjbj.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2temqfyid.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2tdzrtnxt.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bpuslwuj.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2krokkvwi.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2avaoljko.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2gpsasuap.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2glyvukuj.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2npsvqeyx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2tmnzdfhb.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2icnplirp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2bxoplpem.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2vmapmrpz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2dbnmudeb.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2chqbhjay.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2gcmcdadb.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2trbhyslo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2zdlnxtph.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2nmrlxmqw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2mqvegpdm.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2yiynfnsq.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2bawgclgf.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2elbnepyf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2rztijucs.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2leapomzh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2vxkuikwa.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ubkotcpq.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2fxdqoigo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mhudkldn.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2epqzivlx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ndgwsyxc.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pwgsgqqr.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ixksyntm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgulszfy.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2hytdxzzv.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ancvwjov.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2umorcltk.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ltwchcjj.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2jlzytcwi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2tjxnhrad.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pbcnmvrm.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pujkygsx.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ljmtrzjf.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2gbwnqhkj.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2bqxzvqir.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2tbcbdrwe.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2swnkxqbv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2iiqpawvy.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2mzaqwvtq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2wuwpjdqq.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2yoroqolz.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2sjakexnr.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hkyqmwsa.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2pqeazoyv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vxyialqt.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2fzzvqzbs.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2itjczptn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gjgusvga.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2mkkyehng.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2cczbjvgr.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kezamflx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2vovnbugk.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2xzqyrxjl.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2uknyvstm.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2tfhxyvsw.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2shmqeybp.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bzefxvxk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2lswewrme.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2hklskvzg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2zavazunt.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2afcjmkgu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qudrpzsp.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2zpvaqqmw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hhpdymdr.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2uanbpymd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2yhgexmpu.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ftykcqrg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2yflbqpey.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2gqyddrkt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2dqhnfmzf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2bptfgdei.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2vhjdvivu.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2pldzgftb.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2fhrqxhfe.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2qniapaaw.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2fekqjjus.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ylveanwh.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ymcnkpkr.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2fbnoknju.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2schpbrmf.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2qwbfkkhg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2wjdfyyxn.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2kenamysl.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wcqnongp.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ooragqyk.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2pbgpmaey.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cvzufrxg.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2vjvoaawq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mphtwqgi.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gjfmtctk.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2lwanegtn.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2qthblzsy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ihyxjkcd.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2qsdnmpor.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2jrhzvutu.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2aoshesdf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tnvsgurj.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2wxaxevlu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vqccxixs.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2jebfjacf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wgkweesc.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ruciiiat.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2gywyvzaq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2kqekujif.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2kcsnytyt.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2mxvaffjt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2sekoudyl.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2dnvnfdlf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2wiarshfp.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2facmuehc.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2thyaubny.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2dkqoxkvy.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2imxxfgpy.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2vypuxamb.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2jtcdrdjr.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2lyolcthp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2sbincfmq.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2stxinryp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nofbxekb.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2rumefzpw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2eostrxhu.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xsmfwxic.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2gfumwysk.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2tqemnynf.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2gmitvaxj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2xtbxdwpe.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2dobvzciu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2eggsaycg.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2nxfxsgyc.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ovozmxuu.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ljmmvqqu.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2eqzdnggg.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2wnjswvoz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2nebividx.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2tsjtsqjn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ixififmk.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2mnfezelg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2lzjthiie.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2vzecbwdi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvoeikco.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2sdzfxqbe.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2mbzgzuwn.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2tsqwvvpl.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ichxycum.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2ccwbxvxz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ijozhxla.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2kpnsstge.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2qnvthxxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2esnpohrh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2mwugcuyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xslfabcc.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xpyylydu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2slqyofgm.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2frpnemcz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2qplymhca.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2cgpnuzhq.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ynvebktb.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2gbsuyqse.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2lqxqqrjc.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pdthcptb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2phepqvoe.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2cgxrsyog.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pfvndwip.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wlvqghym.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2misqalxz.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2nblqbuio.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2pgbilxoa.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2tokbfrbm.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2lybsqvoq.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2oefxgxny.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ecyetcop.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2uqfbrgqh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2jcekhlep.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2hhbjqtmv.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2cakuobcn.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2iqpkuzjp.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2lmcnubeq.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2tpfpvaos.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2lyxsqhht.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2yowjujkf.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2cbkqpmyl.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fadphbtl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tgviwile.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2khqinojc.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ycbsunrp.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vvdojdnc.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2qumioevs.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2ozqxwhmr.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2xkcvlmqo.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2mmxjvfrq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2sibqiyms.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2dnscrdul.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2qsuugvhp.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2hhejtmye.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tlhevmxx.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2dfwyxglf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2nbkxsrwh.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2atcxiwav.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2upzqvxvz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2hvrlxdsq.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2dfheunbn.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2rnsemawc.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2uvsirlnu.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2aicdyltw.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2pfqyrudx.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2xelulqnf.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2jllcxwkw.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2hdntycan.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2iuvbebns.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2rilkngdq.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2gcqiadzo.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lpwvogtx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cqqpkjgb.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ypxuudqk.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2fxobpjdz.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2mfrrlnsd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2frtsdswk.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2vpuvtvuz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2wmdxoscj.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2sqptgutf.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wjxxubot.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2trcbsxkm.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2kciqzfnh.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2qezrxgas.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2vhukiibs.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2jnibvydc.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2bqevepvc.html


<!-- 参考信息 -->