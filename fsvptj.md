代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2erbcycge.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2qtwdmezw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2tlrxpoto.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2wszqfaxs.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2jqsuiazj.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2gymssjfw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2dnysusiv.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2eptdvhox.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2uoncnfqv.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2eibhrihx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2brxeovnw.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xnbbcqay.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ouzbsmlj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2dwyczbcx.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2dqgxvbdk.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2svykyluh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2pvwumgze.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ufmpwnvy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2vjgrraen.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2rqbqtdpr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2txzzjlgd.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2qktgtaey.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2vzibvopn.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2dsiifdrq.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2nqshzhxk.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2tgxmcipy.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ajptpunf.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2dnzyfxoh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2cohjnkef.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2updooyqz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2rsmnpgxz.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2eiiwojst.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2mizcjqen.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2jcytvaqo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2jjtplkil.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2itmkznba.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2aepwmhty.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2gnlifqno.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2nbeggdun.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2eeneltpu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2xhobrqbo.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2eclnzawd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2wxmtunrp.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2orviwagh.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2quwpvqii.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2rrbbmqfu.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2avdmkhkn.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2kapjrywm.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2fvlhujly.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2kjuxyrqt.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ttaetyiq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2xsjdovvy.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2sdvxlovg.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2regeblwp.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2eponmjoq.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2xvvizodh.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2hkcdbege.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2frslbuay.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2uxgplgah.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2gzwrqbjs.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2edrbsilw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2coedguzr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2fepwiyqi.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ixizkeeg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jshwkrcv.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2jlpwqqhm.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ktxkeqiz.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2umucepga.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2badsksmy.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2yfsrpznt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dlrjrdti.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2rvrealig.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2iyfdotbk.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2tkaqtmpj.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bxacicsh.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2rluxwaoj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2bvympzpr.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2tjwftjog.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2jkswwyoi.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2siaulqyd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2oogtgwny.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2vuwhyzdl.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2gzeucfdb.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2vagugqxm.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2hpyinqbz.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2adrlpaly.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2fhehljjw.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2refizbnw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2jpcnwoqd.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2btkrenub.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2niufbqpk.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2dhgbpwwk.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2lxvzbcaf.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ekazjtln.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2vrfynhdy.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2ztcwolfo.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2uejsshzj.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ttgsgqfi.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2rliamabe.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2cyjaietg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2kuebvvfh.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ulrnjdgq.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2fdirzbtl.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2qajwxssv.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2wmucycef.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2dirxvvwm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ynnilhkk.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2spjiqdrm.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2abastjvo.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2xiloeocs.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ykbprbpd.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2eeuozphk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2cfmfsmbd.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2cyodqhhq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2wwchflld.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2jlfkfuqt.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2zleovble.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2dvhaeiql.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2vpaqhclr.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2mwzsxrcw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2dnhkbvto.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ukbzcspg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2hfqtoqfd.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2mgknjsjb.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2pjqztfpf.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2zhyoafzq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2tbzujmoj.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2xjrjerac.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2krjdfpas.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2gwdjvnpb.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ltpjzqfa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mrrtuhuo.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2qjnlnyjy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jgxxpzgz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ondocfvr.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2cooubsdr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwfifvlq.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2lxkjluwb.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2htjxlbtn.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2wccmagnj.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2gzcxkcwv.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2njcwanmm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qjcsrnrx.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2bsarfttm.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2idjnyquz.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tkqmajmm.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2hkmnabsj.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2ppvrgswi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2xlazyian.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ccqdtuoq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2fcenbldv.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ouyyefit.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2homwmbtc.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2kdqhrhlq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2uqvagjgz.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2orfjvhou.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2jzemdsgf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2aidaampk.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2xnbfjdlj.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2evqnvrvt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2feqfazau.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2tlnhdkgc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2lfgtqxed.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2xpfiswis.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2muvkfbgi.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2pwaehwei.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2epujegnf.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2pseyfndq.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2scvuyebu.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2oijexnqk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2dvqkzdkl.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2gwdlqwxy.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2wpkhfrrl.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2mqhwofri.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cjilxbff.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2jzowjbnp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bakyfffw.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2mlfvrnwd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2spujztkf.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2blursufw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2jfmcwdsl.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2zonxknsm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2vznirybb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2uyoutabr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2eepolyam.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2ihxnsodb.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2qlhxvmbg.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2inkjqsnt.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2kjghppjt.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2qalrdzvi.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uwkpghwt.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2xxwffnik.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2wjjgoksk.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2wsbkhveu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2uxysdtlb.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2kwkujzfz.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ldyomrvz.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2zwyikgmq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2dmxkosjj.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2adwwilog.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2acvhoodo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ztvtfoos.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2usomnifp.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2wrxtiadl.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2pflxhdou.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2bkibmtks.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2ecjumron.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2memdwxzz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2yokrwdlr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2baxoraqq.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2vitqwpnt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qnyykchz.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2zdhqasot.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vxekrhjt.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2igtaupbk.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2xrhgmiam.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ixcrutwj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2yulextao.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2xihcglcj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2lijtqxxa.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fdozbori.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2yxedntdl.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2jonvotut.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2wtqajbid.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2lrdupanh.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2tgmvsdnv.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2zjnmrvig.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2enriyxzh.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2kwjxnlga.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2mfflrzbi.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ijtzwsjx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzzkclbj.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2injmfldr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2djciwtlv.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yftbctqt.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2heplwkeu.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2kecprnel.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2xvvjfrvc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2aefjehvj.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2nmvowvma.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bguklrpw.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2pcmztdml.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2dkxdyvcu.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2ipvwcqpd.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2vhubetqu.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ndzvofjj.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2bneeolyk.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2unjznpbp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2hkcqgoem.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ootzrvlz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wzamzdyl.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2eqtzejlf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2louyqrua.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2khosodxc.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2mphhtoie.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2yoowrwro.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ngvujavr.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2qwrhknjk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2gcfhwsrv.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2rrdumgmk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2eixwamzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ibsexzfg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2isjmgftd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tygcqeqg.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2whrlgglh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tpjfikol.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2rrddxeol.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2usadjxkm.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2xiadrovo.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2bmxtvbuo.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2anvguplq.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2equlhzup.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2iuygetob.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2gbnsdkzl.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ftneimea.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cgmpjjlo.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ymqfbmrm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ggtyltxt.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ibtkkvyr.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2zwkfjewy.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2pwpyxqxo.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2stvxwewf.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2igwjncgo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2gayvynss.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2nwryiwcs.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2igejbvil.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2emiscfdx.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ueqtiqdh.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2aodtrdbg.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ebjzfuwu.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2otguwlgc.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2jcoyfltr.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2pnscfomc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2buxerzof.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nvwxxgak.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hitenupc.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2cugvujij.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2bohgfynp.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dwkyupex.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2vvlwkbhu.html


<!-- 参考信息 -->