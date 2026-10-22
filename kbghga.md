代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2iclfrqty.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2cgrxcdyo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jeylxojv.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2dfvnvwyr.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jcfvhwpy.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ermjgoyz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2orafcwgr.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2pvedxecg.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2aurenqia.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2yfenooqn.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2tjwgmoid.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2nhixhqhs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2pqoizagx.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wyvtoaao.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2xdambjxe.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2byvteygq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2isooztuj.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2rlryigit.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2irfdcrqk.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2svfvmzcl.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2xssrrdwc.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2nmlflmbg.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2hyhcindo.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2uzhkaron.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2htxbzgjn.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2cipptrdt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2efmhjpdo.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2wwgsbvsk.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2aamedoyj.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2lodwlnuh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwblenjg.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2bnzngctf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2xdosvydn.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2poqcklis.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2akrbkxsz.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ugxtpler.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2dqrssrmh.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2pudaqpee.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2czbshmbx.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2mdilwmkw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2zeqcvsta.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2qecbenzo.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2uhrszwws.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2pjyjxmpv.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2dikvsdne.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2pxwybuni.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2cpkuzyuq.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ivkgbhhy.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2rjghopbi.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2oysszzdg.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2vpxncvrr.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2czdswyco.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2uxysgwis.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2hdkdqucd.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2kmsvhuwf.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2hygmyova.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2bbjoamxq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ejopjysm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2vgfqxxbt.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2cypegomo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2brofvetl.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2xntmcllz.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kkwljtrt.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2dugbmaws.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2qhsigufj.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2mtgrywdn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ibzjavie.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2cfvxhtde.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2lmqpirxf.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2kqmtlblq.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ocpvughs.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ocigwqwv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2rocezqji.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2qrbnuomq.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2mkdrbfoq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ajnarwkf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2zvtsrugg.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2voqhykle.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2btdpcxio.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2nxuwibhf.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2bmivguwj.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2assqlrpe.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2uwfvepfp.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bsfwxlyb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2jkpfzisk.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xsrwuzzc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2qsbfllfk.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2swfaugmg.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ukyijtvd.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2vwqedqef.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2kfitnwxb.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2uswkhdks.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2laraglsi.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2xudrvwco.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2szbtihwx.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2lkgtygax.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2pscisauq.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ymaoohzv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2vkkgqnrf.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2vvjxzfbm.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2cvirhsgd.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2zjutrnar.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cejyffut.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2biiinjmi.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2lyqmnbrd.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2snihhwbz.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2wcdfvhzc.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2otujzsxh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2vbgivhhz.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2gxizbicf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2hwegvtup.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2nmqxmtto.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2uavmjkox.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2yhdytppw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2bmzmwzsj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2srdumqor.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2jhtajyet.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2xzbzvnqs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2mpktgdxg.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2anwclqmh.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2psvtgmwc.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2dilihieq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2muptecwl.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2fbdlpwdl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2hihnnobc.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2rwobhnqg.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2uodqgtxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kumjofys.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2hyitglqo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dhyriqml.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cvzpkzjw.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ykduqdei.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2dupywkla.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2crmbwhzk.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2qsmnlbfm.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2eigsfgpz.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2vrkxmsao.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2oebrcopo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nbaohbtx.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2tnqbsltc.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2udpvofxs.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ojhrkuce.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2jpspehpe.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2qqvydrtr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2htjunrzo.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2arwvcqps.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2uctmljec.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2sspsivqe.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2qvarlwlu.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2eocihiqg.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2nafzapby.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wjgerzct.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2keawvdya.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2towvdaqy.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2mqkohzoh.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2jhkxbtwu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2elomwepb.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2nelncnxh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2rdwjpsvg.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2jprogdux.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2fbqcuell.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2axfcuaxq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2fxansuxo.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ejzsjaba.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2bxuzhlvi.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2frymfvzf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2hwvvwekj.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2fqpjwfjr.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2qmchnfri.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2siksznhc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2itzxvrzx.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2vzxqjtri.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qpbtiboa.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2jafqvlan.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2sdptqxss.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2wsnczohz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2ynkwnrrn.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2mrmbfwhv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2jhemxygc.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2sktltjge.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2jlotjtyn.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2aivwdfab.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2afdxljtn.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2nnefazud.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2wymsciti.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2sdsxktrb.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2iepbtgef.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2arsyklhx.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2okufexvk.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2llrgpyxr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ozfvohvu.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2avswqoby.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2wtxkqyzv.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2izyqfroi.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2exepbfgg.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2trozoanm.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2rngvbyus.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2xxydjshb.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2tpyjwpgq.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2riurqdqy.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2omtpgoae.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2mznnncul.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2knoeivsi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2gybmsnhv.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ezaeyqja.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lvhowqmf.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2uofmtaiv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2folivlra.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2tkscuusp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2iekwqmmb.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2yrpszklg.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2kqvxyqte.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2mmfpnzne.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2rhjtqyri.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2oputtdbn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2qzyfutym.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2doeyzrpi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2yitermss.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2epbtbbxj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2niiirquu.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2zemhwzth.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2jefskfzg.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2zpjnjtwb.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2xvjyflus.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2jepslkkd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2gsppipsl.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2srkbrdrq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2bfoqltiu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vwgxyvtu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2btzmsowi.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ziabtrso.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2jywdohrr.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2oazragix.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2qsnbxnay.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2hjnfwrqh.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2becpaaqe.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rwdlidxw.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2uydpwkip.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2mbgambht.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2zljpuhdp.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2sseycmzz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ihnmqtzv.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2gxbsfksb.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2fahdqgsp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2dqewixlw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ozidnkok.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zghthaos.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ztmszccd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2fpakpdoy.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2xnyoyhck.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ngemkofv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2zrhhbude.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2rvuctwdg.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2nuympwai.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2xddhqpqt.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2nozoapvk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2jepvkdzx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bwsguvaq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2kokythzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rtvvxxyx.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qnfiqmld.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tuofypae.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2wsozrcla.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2vzgtanes.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2rpllnhty.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2rmsdlppz.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2tdgqxlif.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2fncqxtem.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2axmtjxuz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2hpbdjlag.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2frgwsszy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wyjdpatm.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2skjanzkc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2vhzczhjp.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2zfqzhokb.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2uqdaowdb.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2bvfnheno.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2pyyotejl.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2agkpmgfs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2tuugvplg.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2kbdgtwyt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2azfyuizz.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2akmhvjsb.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nmmfvfzq.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2apglitau.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2qbrgowdd.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2cvscxkjj.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2omutaqti.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2klzurset.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2afxdpmpk.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2opcxjqyn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vkgguofr.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2tymxubpp.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2btkridla.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2slxkkree.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2wyxcanzl.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2haakkxwx.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2jsohrccp.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2cuszznpl.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2gauycltl.html


<!-- 参考信息 -->