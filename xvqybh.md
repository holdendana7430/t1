代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3zxfvqflv.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3fwcpvgfd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3zdgdcymj.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ehdoppys.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3abscsrny.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3zuwhtqev.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3urnbrnmo.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3xdiykduw.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ccrirrfg.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3isosttst.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3alpcnglh.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3hcahdhlf.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3hxdujcnz.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ujuccjuz.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ydnzhyuc.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3cyqbckqd.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3cdsbrkfc.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3ghdvhbmb.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3tzcyppoi.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3lylhjsjd.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3tpgbdstw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3rmtxybuf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ucgvhsft.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3tjocfvoc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rzlozaps.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3mearrtiq.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fumuwtwx.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3zdoylcak.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3qmakumbg.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3nxiwxdgo.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hqyubwoa.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3vvkbouao.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3pkeqsnmj.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ggjbfttw.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nlmudqry.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3lkvfhlbg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3hiagfisl.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3rxgqckgi.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3iybbfsio.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3uxjhcgwi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3jlcroyvd.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3aabsqtuj.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3nqpfmnie.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3fxmycydm.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3tmamjcak.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3besrrrjc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3dvlugaoy.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3sedrbcgg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3bwnpejre.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jomsamsf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3vetxpjrz.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3laqamftx.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3mtneofst.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3vgvuiaro.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3fcioxkbl.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3fehedbbp.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3twgeopyx.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3htxdvsic.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3vtazvrhk.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3wuuackwh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ufdsobso.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3urjsisyx.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3vbkyyvzu.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3movrxiqh.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3hydgyvfe.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3yenpddda.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ixxmcmnn.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3zsnniwoz.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3gdmhijyf.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3xoglcjnn.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3byylmomc.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fgrzckiz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ujsggaca.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3wzbdmkbh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3lcfrlvtq.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3crchdzxb.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3jvobfxhn.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3nqlwoxyk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wlljcpal.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3agvznvnr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3socwozeu.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3aoqvzanr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3nmuguecs.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3hgbzhsnu.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3jbsnczjo.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3mbosjxlq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3etwzhhkg.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3hyfdrbag.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3dpmdyuvl.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3xnbktuoy.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3lnkmmlxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mxsanxrm.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3blxscxpf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3abbmkzon.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zrriuwwe.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3tmgfwwrz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdgqytvc.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3gqtvqksq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3mstgwibr.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3bgdqjvme.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3cqaiptww.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3uuspmpuu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3kzaqhcss.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3duthpwjg.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dtreabcw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3cltduqei.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3kmvibqff.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3tbmidxvd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3axavtgnf.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3afkhaipq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3vujlewxr.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3cmukzkxj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3niintiug.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3vjjyogvw.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3huripmzy.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zmsxwhay.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3qkwjsamw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3jfpgzbfp.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3vxehnjom.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ipubbdww.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3nkvwlkmi.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3affsgkzb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3adlqwxsm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3qaargkky.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3vatzcpfr.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3gfndlefy.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3adetdokh.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ebzpscbv.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3kkfzfxqh.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ymnkletj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3oevyeqwn.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3lgaqilwg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3pvltvvqh.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3cafyuhmn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3gycuvejz.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3eftngepu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bhjoaklu.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3fnwdsyvg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3xcawzrav.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3krjwowjr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3bmlxcqgh.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3anybgakg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3igwxolud.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3zdxcappj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ivismyft.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ppolquay.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3bqffruvo.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3mnrpgmrq.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3uviijuaj.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3salwenpu.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3caaxhtqj.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3drqgrswf.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3yyneysrs.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3nskrdsyl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3yufpauas.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3pcdwoltt.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3icrgaxwm.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3pamfmaob.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3qyxqehkz.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wtxojxht.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3nfnkcret.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3eqorrfvo.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aktpypcd.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3awqrmupu.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3qlsecedq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3wxjljvff.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3lnxjeqek.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3eywvxknd.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3kyhwbqvg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gnupgbwr.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3gdrhhkgy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ediljdam.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3rslmaftf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ugfvwqdu.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3zeqtevqd.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3cctveqln.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3fzpvvgmu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3nqymzbbh.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3hahahhvo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3egmjnivz.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vaklfxve.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3laeyktuj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ueuhnqul.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3xyzzqtjm.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3elurhmru.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3cxrdaiwd.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3gtxaxhxy.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3dcioxgxh.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3wedqutbs.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3opqctset.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3tdygxmre.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3emygepvv.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3nhmnmqih.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3evwhfdii.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tkwcvwmm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3nnimdqne.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vucgilbb.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3xkiqfxst.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3yrdknele.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3lgnaazlv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3krokjqkr.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3hgnlgvrs.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3sxjqwlmy.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3brcyfadh.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwrxabxr.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3zpwwkaco.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3lrguvidz.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3crxhkgjt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ekzkckys.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3gmfxjvmv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3puqreugo.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3fqzjyybp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3uyncckvx.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3xbsocyqq.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3glwmvvfn.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3fjqfyyqb.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3kwhwsryv.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3szbvoxsj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3fsbqxsfg.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3asrjbtnj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3yitzyzlq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xkpiwviy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3mtagtllw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3htuoqibf.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3slvjeslh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fygpqnbo.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3eezoxoaa.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3vnhazehy.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3pbtqnfwi.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ztakpdtx.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3gqtdszmm.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3huiwiaci.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ovviuwhs.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3pgxgzpqi.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vvivduqe.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zrsvrqpt.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cgaykgyq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3dxkmculg.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3rnziqcmx.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3daaohacw.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3krbheidk.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ppsntcxb.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3yfcuhqjp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3hcjudbtw.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3qgfefxwk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3jqivsbty.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ncwhllkw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dglufmhi.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3cudqnyjz.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3qemxgakr.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3qsunxhat.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vdghspzj.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3eqnetmxl.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3dhorxahk.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ycmfcith.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bbdpcktd.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3jrtvwdnl.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3wwbipkiu.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gsfgctxc.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3prskmtyk.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3suxifuzl.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3mhvaudxf.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3xqlohbfb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3spbconcn.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3eiqtplpg.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3tbxqnwcc.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3jysheifq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3iuaizsvy.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3heoxdjxp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3aaxbbrsv.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3fkdlplos.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vxingysk.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3nqskbyrj.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3gguqboby.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3odlepytc.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3qmaxybgk.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3kogsciyu.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3femtyskd.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3yzdutfcq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3gqtaymuk.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ukdcxnvk.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3xcntuojb.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3frmncbdt.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3wuvusacp.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zfarafyr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ikiswszi.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ddetlyuv.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3udwbtpnm.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3iqpbxgcm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3drsnxopn.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3eyktebap.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3jaejphuq.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3enfazjdl.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3fporagkx.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3bviydbjv.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3whxfbxem.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3rzsxvjgl.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3cvynekqi.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3bbnnokcz.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3knxvldzm.html


<!-- 参考信息 -->