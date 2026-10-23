代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3fmznmtkl.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3wlqmjcxx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vddvxath.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3istkjvog.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3izeczvdl.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3rsjuwnfn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3hqljmedw.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3wyajfiri.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3yohltvrt.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3yjubdwqk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3fctndrxg.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3qrktjfyd.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3dqegfvcd.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ozodbleu.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3xfrpzfoh.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3cklkyxfr.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3khohgpfm.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3lznxhqgo.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3qhczfsbu.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3cgevrklz.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ivlmpkke.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3lxfjozch.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ljfxrluz.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3vkmhznmv.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3tbcrvgbf.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3driicxxj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3nknlplan.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3csquoboe.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3pjtulegu.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3wlhyerkc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3tvydwkkf.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3yrjibbic.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gzpnpbtn.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3icfwqmyu.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vccaenub.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3nbjhkmvp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3joijhhfr.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3apkphbcj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3bfcpwlqi.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ruhwhhtk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3afpgdjvw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3hxzrbufq.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3idwdxdcb.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3maajqevd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3jeslshti.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3hbkafgse.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3oztibxch.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3bcwmlfyu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3sainycmf.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ljfmpjza.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3gudtfazv.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3yeuchdye.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3pzmmvmmd.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3feprytip.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3jzyyhkbc.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3rrzfyxtk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3wknzatnz.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ayidrxks.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3gwbsdejt.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3fewdrhew.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3yypytwzr.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3aofbsjvg.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3bdbenbxy.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3sbgclngc.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3csicdsdd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3eyeigcpl.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3wsokuqoh.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3pjvxdfby.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3rvbpnfut.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3izmdxzux.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3zshffeeh.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3cbutwotq.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3zzcibexo.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3rbkdlcaz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gdpiukst.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3ixqqllim.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ynhvkcoe.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3qpcnlmdm.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3fkckuvht.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3sjplsouf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3jnemprsm.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3tnxyqavk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3wdeuaggl.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3zslwunfh.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3trbwcxga.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3wwsoxskv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yxsghalr.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3ydxinitq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ueajfheg.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3vzlikvbp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3gdmihcyt.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3wicsskwj.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3yzurxvmm.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3llmltlfc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3bscdobkj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3qrzfbaxf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3thlwcsng.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3eetrvoif.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3azoogvxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lafoveay.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3bdqxoqpa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3harmhbqw.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wvlwlgbt.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3uzyrfxje.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3rlgvdxud.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3lggymtqi.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3iadkwbac.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3vkminrsb.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3aqlsubji.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3tnehedxs.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3rtdtpsxc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3czmguumf.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wrrsmhqo.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3lueqnwuc.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3zqgmpldl.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3keqhcgqh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ccmkpsxa.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3masvyxac.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3lvnynwrx.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3oltvbrzv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3dtafzzzw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3seumbhyg.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3tucdxuyp.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ktcwcpdr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3fjmcpygf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hybypoll.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ctifkwiu.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3zqmkhfjc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3cumcqmjk.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3pykwyujh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3bfuhtcjb.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3jjaxkkga.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3wjfqyxdf.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3tccrxbrt.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3vussyswc.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3jcyoxais.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nlysynbb.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3srgfgmpz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3qrswdcmi.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3cppbjjcr.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3iskriuat.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3slcxqbdv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pmxhftbx.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3owjzwzue.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3pkkllwsj.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3kwxlhxjn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3nnjawzab.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3bsasgtej.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3tgcuforp.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3tcrymezy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3clmhtcwu.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3bhnkdcfb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3zrdhvgzi.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3vkqixcpx.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3efqcblrf.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3zlfdiznd.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3xbwraamj.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3qvpeiwjy.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mrnkmzde.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3qlkjmgfg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ujozglwf.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3iuihqhix.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ptsjmnbr.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3eeehephd.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3tcuntrfv.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3eqsajocy.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3yiabzbmu.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bwbhzfix.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3jfchxkgp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3sczfwoyc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ouwhhrgo.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3pbyovzen.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3jhsriyme.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xxxppzzp.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3sxqnnunx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpiujyhr.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3gjqifhnq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3iufacjlx.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3yuiekwzs.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lzoimesi.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3lzyakxem.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vphvueve.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3wjbhjfpg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3kftwfbwe.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3fhwtxrfy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3fzwrbmhq.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3njhumlwh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ogbpacij.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3fqpqlvks.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3epwvypgu.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3nnihbfkv.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3efmhvebn.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3cghgvdze.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3csevpnvh.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3cpeomdaj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xuhiovox.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3sbhtkwou.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3azltpzpm.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3zwsxontr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsrdbcpq.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3caefjmxj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3nlzicpex.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kaxmmwud.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3zwkppysl.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yjvapcfy.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3bxyhgszy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3qwhvnitd.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3zgekvtmm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dqbxazhc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ljbehbxk.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3oyqvszbf.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3jokfdqij.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwrfilfa.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3cqdpmppz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3qruqqlnr.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3tkdtwwlg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3jjlhczpk.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3bqliwsir.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3ufnjixoj.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ezelizmj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3jjcmqnhb.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3hteipwga.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ifhflncy.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3uecympkx.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ntmllawk.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3votsqech.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3sncieuoc.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3oltvqfbv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3hsnfnlgl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jytrqpdl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3dcgemevc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3isetobvp.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hdclxbhg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cbbdvnlk.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3frswvgfp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3qdhgplol.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3vnardhbq.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3nqyeowqt.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3dhacuhro.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3dkxrfega.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3zfzfoigf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3jciymocb.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3evakjxwc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kpkqxcsq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pgrydnwn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3zdvjfilt.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3mqlnlivf.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3dkuoxnon.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3tqjxqtxs.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3kbppbwmx.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3soxqdsaq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3wtvjiwlr.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3dhxptddx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3cgxjrpcb.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3gcokmeuk.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mhoxugzh.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3jtlnipsv.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3zabhogjy.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ovcnxtns.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nbqkjpvu.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ntimuzbm.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3nyngwrzu.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3csyzodkv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kueafbhw.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3wjiyfxmp.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rcotvjvm.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dpwvlhoz.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3cfaxfnoo.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ejdauera.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3tqxjwhat.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3lghfirwp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3hhkvxebs.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bwgeurds.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3eclqswcu.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3wxeejovh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wkcmuriv.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3sijyzaib.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3cokkhgum.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3leqhnuzv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3stafbkos.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3dlcqdjao.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3lngwecem.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3rqjyfsrz.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3xsrmbnxi.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ecvdcnnk.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3pduauhwp.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3zdvbypdc.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3dnjjoway.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3pmtftcno.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3cwjfnzqt.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3djslmgnp.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ewkyadqn.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hseqsgni.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zizwgrds.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3pclntkts.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3jibaglqc.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3caeasgsp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3rnpwovhy.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3zhqmgttv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3xkslrbcf.html


<!-- 参考信息 -->