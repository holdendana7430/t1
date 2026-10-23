代发 wailian999

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3howolsit.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3rxqnkywv.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3damdscoh.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3swvjspcz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3crisparg.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3hfuzsaus.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3fnwrxuwt.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ycluhity.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bsovzuqo.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3kxrgajto.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ktwwgjai.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3bggmuvzb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3mmubjzpz.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ctbndecv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3vdlnijrl.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3xwhccfzd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3wwrxympa.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3bjyexjer.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3qqxfttyl.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3blgubvzz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3hnttbamz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3rqbfutxr.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3fbpklush.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3sjjwceab.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3hicyimra.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3cwvldoxy.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3zrggdqtw.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3etnhzbaw.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3jivvazxm.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3lhvkgnek.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iaobftsy.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3asjzvvyb.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3dachtuxj.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3thgqyuuj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3gbshhuxi.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3pjgwvels.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3iewsramv.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3izhtmqjv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3vuhopprd.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ooyfaauw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nvizdqyi.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3mwfthxdo.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ltlgxtbu.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3aypwvoya.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3kkopgtsu.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3geumhcse.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ibaejifd.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3niggnhoa.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3ycntgtwq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ppgwrsyi.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wdzgzgji.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3uchaklol.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3iyucprkl.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ujmxlbqf.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3cwcqoeiu.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3sxtwztzv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ucqtsjiy.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vwziwnxr.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3sgmqoyip.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3rbgasotu.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3sikdbmex.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3lfcqnyyz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ynbdyifz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xqcyhhqo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3hcxxzblf.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3tghdifzl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3caajdcnv.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3zaqredfj.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3bmosvzxv.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3zczhfouc.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ebseecla.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3eclcqpta.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3qbzhrufn.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3mlizjpes.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3sjppyybj.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3bjkduozs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3eykbgpyv.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ropbzjmn.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3xaxrlomn.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ecwyoxui.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3tsaipdrd.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3ttjccito.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3zubixxji.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3fbttokgj.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3edqvkpje.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3hbtcvgkk.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3zinbnocp.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bvtatdzw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3eckkumah.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3ffpgtwev.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3pepvzujy.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3yovrepit.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3nryvxian.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3cbqjcfas.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3zgvdzkyd.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3shyrvrsd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3wcfdwlur.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3krgvkgrs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3kcatppda.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3grziyuef.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3wltzmqta.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3wtbixtnw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3unnpkpit.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ckfbmaqw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3atwdruph.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3jkhxomwx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3oofrojdl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qdwlomia.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3kdniddnq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xybnwtin.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zthhepjx.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3bsykrknj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3eblfynci.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3aflcidzb.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3atwuwzui.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3jbrditaf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3lxyraswh.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3vgscksfu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pewcvlrj.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qdmroiss.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mxpyqgaw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hyvgimxb.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3bvswrgqh.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ckrmvbxe.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3zlwthxgk.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3jujihoha.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3lhmlpkyj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3mslpclbr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ftxfmpgb.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3uruzwnzk.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3lcknzypt.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ajytlysx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3vtijwiud.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3iczhborx.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3smmwexna.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3fanmnilm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ngqsdlyo.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ckwvbklf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3kxjvzfdd.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3gdykfesg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3bmojgvcj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3zqrxgahs.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3dwyoayef.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3rmtxpupw.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3jqklllkb.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ezicpmtz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3dqgyzeaf.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3uedtqtsj.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3zrwtattd.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3llfhdirr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3xbpebydc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3wdbpskwx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zqtrydfd.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3hcmbjngq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3mwutrkpm.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3vjwcaefb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ucstmono.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3pkrdouze.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3nptwbsfb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3puhvmsih.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3dtatnjic.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3jygxghux.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3qsvunrtw.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ejyrspur.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3mngaxmiy.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3ylvrgxfa.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3koirignd.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3oiagemup.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3mopxvhio.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3rcigrzbr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3uezqqibr.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3xazqiymw.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3mvdfouun.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3szfswpdp.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3bvkukosy.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vqvxwzti.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3wmpejere.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3nxgdqkic.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3rfjozvlo.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3ekbpluep.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3xcqmuqle.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3gcwiofpe.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ohzuwfol.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3aqplmkdn.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3zmnacjbf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wcgzgptw.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3nkxsnkgf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3porergnl.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3jxtugbmk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3uhwzosrf.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3cyadvqbq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3dcilzzyk.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3qkjzldzd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3vxqvqyqx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ztffqllm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vbzxphtq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ezewzitn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ghvqpvlh.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3jbkyonae.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3bzfigkpo.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3dvtynjdy.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3aginbmfy.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3egsoulcl.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3mivzzgxj.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3idifsylg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ehendnqc.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3jxgctbrz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zeminwyc.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3zanklbku.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3djopeclv.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3orargnvc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ojtyszoe.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3iuyyuilk.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3qxauqttd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3bvhnyedf.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3kybkgrwd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ahzepifp.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3vdfzczcr.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3vtdiosyr.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3iplldfyd.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3caoogoyk.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3ckkqftot.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ctsvvebw.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3uxkjmxna.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dimvabhy.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3mclhjlqy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3rwdfoaom.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3riymapsy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3grqsfvbd.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3sgqhpasi.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3bkfpgxwl.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ojjhvrxi.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kiubvstb.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3eiujipcd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3byoeelps.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ramfwqmk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vaojjeat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bnbasflv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3shnngugj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ccytvjql.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lxnuccdj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hpowisqp.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3unaavjwd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3yvjuwnvs.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3fvvlswpr.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3lsssismr.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3eqjrengk.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3mgomqrkq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3qxwzlndd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ssddkdvn.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3nkrmkdpt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ursygtxr.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3yyohktlc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3hxebxiba.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3wmuhnwkj.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3guxyqzkj.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3jjznlffs.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3llmofmwd.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3aqysqegk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3phjvtwdr.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3mwlaqneb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3riotldsf.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3dpdcekgk.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3pghmltdm.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3afgwgmnw.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3wwtvmrwg.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3phtfvqfi.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vvycnpde.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3cplyrafc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3dxbbxtnv.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yvhklxgy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kalrobht.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3fvukrprz.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3glvriamw.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ntlgwcex.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ybtryjec.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3vbcxveqw.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3dfmzztpq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ppeijcyk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3phlnbqlc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3bbpnvrjs.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3xebqpjzq.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3spizmtet.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3dnfessvh.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3igvosusn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3aonmdxol.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ioxddzbj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3javgejss.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3idyzozkw.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3zddhxppx.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3dtbejdat.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3qzqnudnd.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3guynisnm.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ddvpwbdm.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uqcwsmww.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3fzqtckcx.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3exvxhoml.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ztwolltx.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ylqrzxle.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3yisgmubv.html


<!-- 参考信息 -->