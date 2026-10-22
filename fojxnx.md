代发 wailian999

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2nacxxhye.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2fgpykacz.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2vjcpmofh.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2swgwxmmm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2zfknkwpy.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2kqfsowwz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ycbhinvc.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2qepaftgu.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2mdcgzxaa.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2lrizvbfh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2bgbmseba.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2kzwnlchg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2wjdcxgmp.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2zpyxkovs.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2tjpqcrlw.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2umrtpuij.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2uirxwakn.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2vihmitac.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2duisknoa.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2rrhdepgh.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jbdyrhet.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ntndrwdo.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2wwtwkccx.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2xrwoaglx.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2wdgbocgo.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ajueqrzo.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2vhpglpjo.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2agodcavr.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ewxxpskx.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2loantrcw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ugowwmkq.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2cccewqhy.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2xavjydor.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ngafltpi.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2dzjdtwjv.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2mkqtespp.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2zsvuqpct.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2gacdtoav.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2aegonvvz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2vqmponoa.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2univivcx.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2dbxnwhod.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nwdlavkb.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2tntpaqed.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ccitooao.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2nqjitwgn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hqwrnkfu.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2byofzpkz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2eyzplorr.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2jjfkrirc.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2fpymcxpu.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2szedspts.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2gzzvspqz.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2epksvdgn.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wwuomykh.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2fcayiend.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2lcrsycse.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xliareve.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2qyeikzjf.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2svruihvy.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2hobkmkzm.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2dotrwgdy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ivmcepzi.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2lmiibhls.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2kdmdkcas.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2izxlcngm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2erwanpwj.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2iejrtieb.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2pzbpqpji.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2hlyrxvmx.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2szgqemqd.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2wlywophq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2pxgckyzi.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2urwlwyhk.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2cwlxlmtp.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2vydgqgwm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2xddrqhke.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2tumuybjy.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ciczaogw.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2dntlgxap.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2rdnrrkgs.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2dwdlidwj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ootxnzcr.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2pwzlymun.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2vrzgstop.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2xbeejmtu.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2qmogrzsy.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2bucttfgx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2jdwsicsg.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2teajraze.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ffranyoj.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2liedluoe.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2qgkhykia.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2xypxtqlp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2zobtrvwj.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jxdjxndw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2poyzfekk.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2jfxlbsfk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ilkuwdxh.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2jxatlksm.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2dadjrbpf.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2ksehyizu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2dcfcgwys.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2smugbzyg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2rrsuhqvr.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2lpvvdpda.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2rqrqbros.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fgbvoddf.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2shpfarvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2azfxjkom.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pucqvezd.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2qusfozfg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2hwiesfmv.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2esceucad.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2njfyvpge.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2dzzvceem.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2nkqhtpiz.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2orzzkhsl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cktraxdc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2srfyfdya.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sghwggng.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fstalxez.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2cthcjblx.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2gdawyafi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2exevjndh.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2kavfwboe.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2crmmdrsa.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2hvvnrsfj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2gzkdkiqu.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2cjonvnwk.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2aelejxnd.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qlecaoaj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2mxxndodc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2oerfeslg.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2yatnqfsk.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2xnwocdef.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2qwiwyhpk.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2wqrsjtpo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2rzzqvnug.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2abuywmlq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2bcbpodkq.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2jvkytqgi.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ybfxzkqs.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2klcsfcgg.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2mruumzdg.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iiiqubbz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2moitmneq.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2jsybjzmt.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2shszrbpv.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2vfuvlxrv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2pkxlqahc.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2qzibpugh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vlbxlbtt.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2agbbueht.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2xxpjwjtp.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2tiviwvpq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2nzcdslqi.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2kzdoinvo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2hddyuxbk.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2adffzhir.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2fyusiheh.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2zliyjdae.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2gcqtwqwr.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2cczqehyx.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ytqkiycb.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2wwezmgqn.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qclaqolo.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2jmtzakks.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2mimrkrjm.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2putpronb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2nllxaccb.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2nvefqbbc.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ksnthzkv.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2zszfntsn.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ivymrwhg.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mgbpxdvz.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2efuoefud.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmuxtkta.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2crkxiqrw.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2cmhxbpte.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2uaheiuir.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ckjkxqrn.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2acogrxvi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpsrqtys.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2nekdibya.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2iapucbwk.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2lnzgwrog.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tadlhazx.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2eyvsrhgg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2whkwogxb.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2cqtsmfov.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2krarkjrf.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2paiywdrv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2kjohnpcf.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2bolgdsgh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2xeltrove.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2tfgbmrio.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2zyxphcrc.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2dcbaqurx.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2luvgpvlu.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2gfgculdb.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2broybkls.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2awpdfgea.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2nazatdur.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2emlrkdvw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2fylrglnn.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2rkbwxdly.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2miaqlgma.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oxznxopk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwhuwidk.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qvtooala.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2qjmkwkmt.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2hnyignsl.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2qcvfrulw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2pqwbaxws.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2zfcoxvja.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dndyyffs.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vdbskkvp.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ixijajfy.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2xocgliuy.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2yjkpddor.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2uhbtnbsq.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2autbdvvs.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2uinjuhjl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2udavsvzo.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2cnxwnhat.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ynkjmscg.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2kfzqsgys.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfcmewmk.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2enfcvblb.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tltqnjwf.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2yekvmsfl.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cycgsusp.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2rucgblpx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2xaewmnew.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2hmwczvor.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2nvzqwxww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yxetekwz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2aiwrelpa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dsjptdwz.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bkwbsyla.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jsjffogn.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2posnjaon.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2pashnpwf.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2mnvnmbmz.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2efhiycdj.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2dqejjzlg.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2fomnfdpk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2tbukibhj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2cuyvnaje.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2qhcewdub.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2rssjjpzl.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vsllnacv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2gkbqupwt.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2rhuysqrw.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2azrsivyx.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2arsrzxif.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2lelnluto.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2rlfcodoh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2yxdmlmbv.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ppmgqhtw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2qxkdhqqf.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2aqduwzrq.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hystsbpn.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ncgadmko.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2stvugfed.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2mqmcjixq.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2fpeggocc.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2zomkfiav.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2yfdgsidt.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sccoqohk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2sghdocfi.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2amqcjmta.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2qevgpoiu.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2uvgnurju.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2txqppltz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2juegnclp.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2itgytpot.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ozxbsnzq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ujhmuofu.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ndsmrcma.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2zfuqympu.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2lzxcrqvw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2zytkdykq.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2tcpnwoci.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2dvxgsvnh.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2porhxutj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ndkyqyfq.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ywccxmlt.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2jeesrgui.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2wxyqbjzi.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2rbqevose.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2uyhhdwwv.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2bqqxhdej.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qlvephib.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2emyoffcv.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2bxfwhhgj.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2eduqzvxd.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2zskobdol.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2rggtrhml.html


<!-- 参考信息 -->