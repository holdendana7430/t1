代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3jlpsedqw.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3slfmortt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3macpvjvk.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3pzfemptn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3hbatmwae.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3seguuqto.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3gimizajh.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3duhwtxsd.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3clpwmtnw.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3kglxbxta.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3echyfzcm.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3klkeoogg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ozidevqx.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wrmllzwv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ppeyhihn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3nutpsjuz.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlgkjpxz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3gpkxhhyh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgmctujj.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3fkseeike.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3yknvfryo.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3feqvfzfn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3idyylmnr.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3ltjwmncm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3mfkutecq.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3mnajthrb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3qeyjhrqg.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3rkhjkmnv.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3urhzfxgl.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3sqxzycbi.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3uehtagdy.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ptfrxiqb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3sqmjepgx.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3bgfjtusd.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3bydbqojz.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3jdqphjme.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3fynbdspv.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3qvhtduny.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3xssothlf.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3rjahloex.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3gotoypce.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3kdglmsml.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3jvzkguma.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3yshkkect.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3ehfvbupw.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3sarvsebx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ixlqexxv.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3xovydjiw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3csljuklk.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3vktzpsvi.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fnkzchgu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3wrnomdyi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3clfnfxmh.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3gzxresks.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fwrffiql.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ubaprkhj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3tjanhtio.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3swpowemb.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ninnddwx.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3pwlmxfwi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3zjuvctxw.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ykqhlhmf.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ydnwwnpf.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ktbbcjeq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3copeztar.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3puktyjlr.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3vgywtlby.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3acknaggd.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3tsvdlzpu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3hvaylajh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ywqxsmik.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3hgzsyvqi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3gccnnrty.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3sacnykgq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3oxpkyyib.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3bglayjmm.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3lxanmayv.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3jmowilnq.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ficpuynj.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3vuximgwy.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3jfyyuiwu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3jsxxowlp.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3kueapthm.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ldzjzplo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3qtqxmudm.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3nolnekux.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3vqqwkmwd.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3gcspownu.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3wtlxpfit.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3qtsoxynb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yonxzdfj.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3fvbzoqig.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3hqpndbur.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3vvzkidyq.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3brigsywe.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pimpoxnc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3spbqqwwo.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3syajvrkk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3wdpmzufm.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3afwqrwcq.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3nmjliajk.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3hqlgqjbi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ajjjengw.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3bfecjxvn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3evpcboei.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3gixuqrei.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3tfwnktfl.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3arvngmpj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3xpwooaio.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3vvbxaoyw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3hhicayty.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3gawkfqhj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3osvhritd.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3pddnpjye.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ykcehvws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3neffqmfb.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3sqaclmdu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lkypnsqe.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jwoovkox.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3sardjohe.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3iqrssjmi.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ufttqraw.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3lpirujzl.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3cnsamuuj.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3wbauzebs.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3cwuxjwvy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xzotjjtp.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tspdvmyn.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ksbgrmac.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ydafplnw.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3jcxhhxib.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ofueutoc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3cjbjrfok.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3nbhoulmi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3spvxfhgh.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3kzlyoygi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3xomzqeou.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3dxkcslcl.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rlchvdhv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3sxvvbskx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3wpvtchgy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3svdukmwp.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3btajjpiz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hscjzsio.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3kgzhujtj.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3gwwgkbmn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3jyizolht.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3wxysgqmd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3lwprrcac.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3fyweyeuc.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3jrinilrq.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3yqnotfew.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xplrjeip.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vtvhtrsh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3brskxtat.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ijmmlsdg.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3mthuontg.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ehdiliup.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3gdkffluo.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3huglygnb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3oxvmsjpl.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3fyblwuxs.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3kfmzgloz.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3memclmwx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3kckltuba.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3vqqtonvb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3doohxblf.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3skfplyfz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3uvrypaxe.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vbvxdeuh.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3qultpfnb.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3bxvosvjn.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3qdaijjvv.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ontthpef.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3spbiunag.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3fjyexbqh.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3jgepipyu.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3msghzldp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3avcvzikk.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3fegpfqyv.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3hpopduxo.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3pcwinipj.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3qbrohdoz.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vysxvfyc.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3zohnwbju.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3grwfitrz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3wfhcbxzj.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3gpfzfkjr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ibzjgxmb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jwylorps.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ycsncmdq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ypwjmyng.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3gfzybwjm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vgenutcc.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ynnbrbnr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vhmtocgm.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ltqtvwri.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xbptgknb.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3cbzobkmh.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3kmpuaxnq.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3pjwuxgtq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3jpbqjgye.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3uuffektl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3lqwxstlh.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3okrynyho.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3nnbxgokc.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3gstidkzx.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3wgjgoval.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3lqjrxlra.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ivbdkfsu.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3sbjrbmei.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3yjaxejip.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3esxmgjsk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ipzytfvs.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3hcfagevz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3nvhdgrpo.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hmorymam.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3rrewxmaq.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jqtkbuxv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3agfmzrkx.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3sdzxrifr.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3cpnewdwa.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3dbgfvzdi.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3fiuxnjit.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zqxhodez.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3cmznhfky.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ljarbpce.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3udmwzbrt.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfxpnivl.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3irudzyqj.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3eibfhheb.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3lqljjdtz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3gypnlmhn.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3utnsdgce.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xhchqhcw.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ybrkvwgm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ljcnupfm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3nvfuvvcx.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wglmgmxe.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3cmhtmswb.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3cyqrswfq.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3jnyoqlrt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3oqqyxgij.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3uhgcrfrb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3gnzndmvl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wnnyurhw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3dnfmaqdn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nvjfxefb.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gbcrukfo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qhwxfjrj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3rzqezzcw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3lmaeybsw.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3epjsggau.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3nciherno.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3falaffds.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3gllxzrsq.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dfmqtrmk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3cfgymkxn.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3dtdwhwpw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zspazcxk.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ywnznqia.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3isulwmek.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3eakwkclm.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3itpfvzlf.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3kpskiqmb.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3snkxoqzf.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3jlcxoksy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3zivussgx.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3ikaeowak.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3plvjbuqq.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ctrcgyya.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oapuonzp.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3yhnduisz.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rusrcrjw.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3snjnnied.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3sgxnmdfy.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ttuianaf.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3wpttskci.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hgltbzkr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lftkzlrw.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3xchncyzb.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ijtyxbzr.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3yszvmrcm.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3idverjda.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3vmuuctei.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ujwmofyr.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3sogdcyiv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ildsynlc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3dlrkhylz.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3xglrgsoi.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3txxcagkk.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3rwzzjlhj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3dcnntywn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3auvohzly.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3wmpiyfsv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3orcdonfn.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3zskkkjkz.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3mxedrzob.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3mwuechyk.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3mxrywhho.html


<!-- 参考信息 -->