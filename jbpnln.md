代发 wailian999

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2znmjfkzq.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2mttnvbkr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hkybhsmm.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2niuszjgr.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2lqzjxtns.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2rmeysbtn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2dexerywa.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mrqymlnm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2ohehuyhz.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ethfahpw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2qqniaiei.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2sgxihaur.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ecahbnqz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2srmvtswf.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2qrmjzcyu.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2irtesvor.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2twfhtcqi.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2rjrbljaj.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ldyvobww.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2jqagmkbx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2gekejhet.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2tsgrxpph.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2vcdknurp.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2hvlbyjst.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2cwlknmim.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2vwnvawky.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2olnrudht.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ajlwwwob.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2onzqsyof.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2xrhwqote.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ykilrqyg.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2pdmbqazx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2lxnrmzjh.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2pxncbgaa.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2zxhopnxn.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2lvkbnudn.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ggrlxamj.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2ovxcjeap.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2uzhpctzt.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2khdfwgwd.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2viygjnfy.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2yttidwmo.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2qouahbqi.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2vgmyglpk.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2gzvmyhdj.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2dhwmmssv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2mnqbwwcj.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2dtvykxxz.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2bbjwhfcn.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2fxkkkxmb.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ampaagvg.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2kqiehnty.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2yiiggntw.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2avjfbsys.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2kgcvoeyi.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2sasrxtil.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2viscoatb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2rqwdkper.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2idgdxcrn.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2okiwvnvp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2zwmeuugt.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2zuupyajj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vmipvxiu.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2nflgmwnb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2spelaxyl.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2xbfqpyxx.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zirzamnb.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2fkqnbzvh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ftmsneko.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ddymtumy.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ghopneoo.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2sucausbt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2cdqsvcoq.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ddewioay.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2dubxcnhr.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2yxcygbci.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2kcvdumgp.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ldupcpfy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2kbooydsr.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ozmwqdmn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2eurnupky.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xkzhqgiw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2dhoawhcy.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2hqqhdoqx.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2csqdtcwx.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2tnialkum.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2afdjejls.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2hxnzoxak.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2wshxfpmd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2mikfdqdn.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2hecmnbgv.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2yhnwyrrz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2wmhosegl.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2jiogtqbo.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2yjvkxsub.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ukngcaac.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2tfhgpjog.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2lqewjvnr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wqvnahgq.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2xpxabbvy.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2nzmzbjgp.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2gpctnwqr.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2mkqrqmvy.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ptcovzuy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2kbyqqjjy.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2mmfghjfx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2kcbcpcgd.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2wxcgazfr.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ajatdprz.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2tduoexsc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2qudspaqz.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wnqfcbad.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2zfxovgoj.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2culcrjbu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2pnxgrblu.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2utfaqmyo.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2gikfuair.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2iwvesloh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2qtbqqqwg.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2xqazedyu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2znokrkvz.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2dggrwqsd.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2vwqbhtrh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2siextezr.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2tovcqwau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lmtbpbpa.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pjyadase.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2lnmluddw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2hkzcirqn.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2twrlqhnt.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2jntahkzd.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ihqkhfzq.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2lzogunqs.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ayrwafjo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dluyjlur.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qzpcyhlz.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bsomkkhl.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2apvsgbdd.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2txncwpdu.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2bgkpllpt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2bziowmny.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2odoqjygw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2jryxzevh.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2miixpxhg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2nwlspiyr.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2tbxsiacz.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2fhywgylt.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rdeqsdgp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ihryfuho.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2fhkuvmmo.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xbqsdyce.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2kdztwaak.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2dmiagrao.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2dfbvjidf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2bjznhnft.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ljpcllft.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2gqvrzuip.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2dlngijfp.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2hfhwjjdu.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2nkuwafbw.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2mbtydzre.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pqcbpzdh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2mktntebg.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2gqqjmxzy.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2pfugkpvh.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2kfvzyrul.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2dqoadjdz.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2qsyflhqr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xnikfsoh.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ycvabxly.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2mfipzabl.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2tyfbupln.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2fwndjlli.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2iytviyzz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2kkwyrvra.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2oqukwuwp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2scnruzbc.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2pirjzjow.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2lnjhilhg.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2dmobyuvd.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2quirxqhn.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2jbpqhagn.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bmvhikjp.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2uccbrjnu.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2hhtmvxqz.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2mjdcyzhv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2qjuicehe.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ssawcqcd.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2cnypnerp.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2uxvkbxqe.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ttyjkreo.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rbegddfk.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2cqyewmrv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2iviqfspo.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2jthpxjqp.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2mtmdbokn.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2mqtbicvh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2viuflbjl.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2keyfjgzd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmfkmnjm.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2mdzbozmq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zbkgkikt.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2yhqvxush.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2afgbijms.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2vgmzavrc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mmasadyw.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ftxrrxfw.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2tuskghfn.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2fhjxgrhv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ejsngfkw.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2yqdxtpyj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2kdiktayx.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2lihydwsi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2njlyqhsw.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2rpicusaa.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2bltgsmmc.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2uzjsoevj.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2nwwgyyfi.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2alpwupta.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfufebdc.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ktwlerbc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2xexqdtzp.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ncwxoyit.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2mrtzoegd.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2pnvjcwnh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2enujjdhk.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zzliowib.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2wxuugeql.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ntmplrpn.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ihvxtuof.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2sqqdxjem.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2vhfrshsz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jacqwjef.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2eicxcnzy.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2nxoxodrm.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2lfgnlrsh.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2oruvvajg.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2jikarole.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2dfquvieh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2judljywy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2frukpzwh.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2mpekaozz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2btwivfre.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2zdrznxqj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfjerxak.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2eygmnqmw.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cwxpskzf.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2esummkvw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fkhwpvwy.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2gginchvv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2uminonkc.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ovawjiuo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2mdrkimrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2anglrurh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2nfhbezaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ejwlbamy.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2quslpuad.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2izregjyh.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ngyfsowv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2yyvjtwsz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ywdacrde.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2rpjaeaim.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2eqlcnvrx.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ythyqjen.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2irxcttoh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2zfiskure.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2rxbxvphf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hhliegyg.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jylynris.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2gszkifag.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2jxezvcih.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2sbwgoiqr.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2baxdzgwt.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2mfdqfqsf.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ooycsgpn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2uozdxmok.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2dwxyaexf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2dlmfmrzj.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2pidubuin.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2cspachrz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2mtbpqvfa.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ryvwfevh.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2kuzwhncv.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bugslwyu.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2jsxsnngl.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2tobqvpmj.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lcgnsvsx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bpjojhfz.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2imzrwqdv.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2glqxdjtf.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2uucrnfnz.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2tgniczdj.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ydpkqkee.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2wglabjdd.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2dbscskze.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2udjrntrl.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kkdcqcsi.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2uiayqwlb.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2qvovsfrq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2mxiqxvlj.html


<!-- 参考信息 -->