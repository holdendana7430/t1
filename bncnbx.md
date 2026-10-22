代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2rvzlwabs.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2pliaetkb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2xpwqsfoc.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2jxhsshkn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2rrtnhmlk.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2lkrezfnv.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2tplqxgrl.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2gawitwqo.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2nstneayt.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2tneafmxx.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2drjfngkx.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2uzcslxsf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2dfbohmcs.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2hushkswx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2rvyiacnh.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2yoevogiy.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwohtqfa.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2gwfxdyfg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2cmwxukrw.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2xijaguvd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ekjefnhh.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2kziwfnxj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2hzgcrkqv.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2utkuvhwo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2bspzuzmi.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2kjovzlvy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2jaxbvmzo.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2jqjsvtlk.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2hvxmjjtr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2pgulnchq.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2orptlxme.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2mlhkucfq.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jtuijugk.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2qqdzmcsm.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2kjbdjjca.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2elhqpihq.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2dazsvxss.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2rubhjynq.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yeauacrn.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2wieslxoi.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2vzsqugmk.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2lwhsowad.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ujoirzzi.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2xqilkdar.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2zvewsxip.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2htmodmcq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2aebtvxne.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2tgfsvrmk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2cnmhyrad.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2eoifacti.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cmukvair.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2qkxysvyg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2stiknkjq.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2biueyfmi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gpadqide.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ntaurlag.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2mmwndzna.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2vvvjvvun.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qsbuzuyr.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2qrmndznh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2bnbyfbyo.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2neqvzgyz.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zncquoqa.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2mmezeesh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2nucvooia.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2umvfrryq.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2czhppeag.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2bvjpjqag.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2tsymymmi.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ivwjqhso.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ykammhsb.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2efdlfjda.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ijadymvg.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2rnichuvj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2fzexgobj.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2grfqxvir.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ocgsupxf.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2bwtdmecg.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2wmgeuojb.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2jgoqzcpm.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2qxtylmro.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2exiglson.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2xleqobvu.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2fufgpilj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2jfmjxqhx.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2hjismvrz.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2zxfdwaht.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2fxmpbazb.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2cqiekuuu.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2zyjsllud.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ylpyximd.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2jwmvxfod.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2erivqgwe.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2zuwzsrnu.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2nxyoacbs.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dzkkbkyv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2szhssvzs.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2pcunklhp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2bnsqubuc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2dzyxbfje.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2cagjsgcr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2jpyoirmp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rwpqhsqt.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ucjxycvm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2bqzonjxg.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2lsqftryv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ppbmgyhk.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2afejwkff.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2engmrmoo.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2cjbcwyxo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2upmpytqc.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2uxvijdjr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2sxebajll.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2olgrlvdr.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2lmhriher.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2skpywyzl.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2nybxktxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mgydnkln.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kybiwwhu.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2cdjlykmi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxetzugi.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2eowbtnqs.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2pninghaq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2wksdffjn.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2dtchgtde.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2bftmehaf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2yxsskvtj.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2dbsnrjrp.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lvcysbzj.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xfudhgoa.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2ztdkrnyn.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2lyrojxdc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ylcrmjkv.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2tcnrbfqj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2xplalafp.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2utvcvoyo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2mdlnydrn.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2nmlglcnt.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2cmvdfwig.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jbprmzjg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2djaqypvy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2fhbixqdw.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2pxinmjlt.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2vnibruqs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2coxlihlr.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2vctiauae.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2mbiedkno.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2wkbtqyvf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2eodhgoxr.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2ixeeqakz.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2vobonpya.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2cgfwqrci.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bwiwwhqd.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2uwxayxwc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2wfpqgkse.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2dyzmtfzs.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2sepcepsg.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2aprafpsg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2tqwxcyem.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2bdvaynyw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zoiuvfwe.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2zgelpxvi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2atvhhfjg.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2nhztvvah.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ukyydvle.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2objrmdrg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2vhvigsrc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2mfhrbqwo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2llxzevqg.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ulgjohak.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2weeivrqn.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2nxcnfydt.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2equqpjva.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2meosdzcp.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2geifazxp.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2rbpqdbvf.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2tgqdqeze.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2iwzvdieh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2osofjqpe.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ljpeznco.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2gzjdbkic.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2sviberhu.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2zyloffnj.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nuvhvano.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2rmnbvgjl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2wwbaqlzq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2sgggcaap.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2rgaeicuz.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2dvqgxiha.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ohwbaltw.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2auvwmujz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2llluiyqt.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2foeksric.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lyjkzysk.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2tzicarzv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2osrdbmon.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2bntpweqv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wdnrkjqp.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2tgebdfab.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2lmmnhcku.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2jagghffx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2aujkoxfz.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2daradczx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dvdowfyt.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2pdhvwlzk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2rvvyirvz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2plinowvo.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2pbznpump.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2lafvahyf.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2epsbzjjv.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2uprdowfd.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogjpswuj.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2grehsqkq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2qqvjgykq.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2vtogyjma.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ueeeybzc.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rdqyzyqf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ufschqdn.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2yfnkeejl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2utujotxt.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2kkdwuksb.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2mntzcvhu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ylyjiirw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2xncuunti.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2uohcdczr.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2neojekku.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2eljdkqpc.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2fbscglhs.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2fvzbytsk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ugmksifs.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2edwdvwms.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2pzmzegdh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2yxipojzv.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2jvzwqwnd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2qrpvziym.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2cnottmua.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajlvsvqh.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2vabwcfhn.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2yksxagfz.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2gagzehyz.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2kfwmhgtl.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2eclvudhc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2hzadmokz.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2urbnbzcl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2zdeahypm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sfkceaoy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2mhwjjvzo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hccbvziw.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ytsomdvq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rscpfxnf.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2qtftjbic.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2mjjjfvrr.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2imatspxl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2hathefbz.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2dvjaqdny.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2hmgqevns.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rmgikqht.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2fgkdhsuk.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2akesqvox.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2waqsxjit.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ubpxljcs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2fcxmulcq.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2teupanrd.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2dpicivjh.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2savqfrjt.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2glceyhut.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2nvinpkir.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ufugiwkf.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2rrsquoeg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2suvhyxzi.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2imcozsno.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gjbvnqkq.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ozhxqgso.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yehkdlbj.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ucsrunvg.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2nxxguoxd.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2uomtpimv.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2cnysobzb.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jlmdnyqj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mktktuzb.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2kxeeogqc.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zzalvsvi.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2elqloefm.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2hblkmnkw.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2msuvhrza.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2kukryhpx.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2kquraijf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2qegjbaxm.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2kbousvwc.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2crxjkopy.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ezlpukug.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2viflrefk.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2raukdkmz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2ijrsecbn.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2anshcljm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2anzsifqx.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2waenlaav.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2aclfukfl.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2ovnnlahz.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2izjyvhtv.html


<!-- 参考信息 -->