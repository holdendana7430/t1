代发 wailian999

esac
来源：http://www.52xcode.cn/Article/details/gt2myteaikz.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2hwoeqcin.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2iqnzkijj.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2wrtbsele.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ccdmunpu.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2fnshbmmi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2efjyotdk.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xzpmzjux.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cfxgkybq.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2aywknuep.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rzktjwvr.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2gpnnmagh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2fbgxyyyi.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2uwnutxvx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2madxczcb.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2bkungvvh.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nyeuzfui.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2uannqlzz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2buifbjwa.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2hppcurns.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2stdcwqnc.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2sxjgniot.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2jgubzrdd.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2utbsonei.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2yjeshtgo.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mnjwwjek.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2jaruciuf.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2izeeywoo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2imliwiyc.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2xqnbcypm.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2xqjmcxxf.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2hxabrwzc.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2uoqjjjvm.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2jbezofkb.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2pzjtixjq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2koltwxaj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2palpeupo.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2emejwpag.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2kyhhzfqj.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2atnvthnz.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2akzftrri.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ymjunzha.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ixioacwj.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2fflrkhuz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2edqqssjb.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2yazbdqam.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2miadenck.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2onbgjmga.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2jplmtzgp.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2ackcxnts.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2jkmdanmh.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2kfizujbp.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2kxswqnyj.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2mpqupjwu.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2qofhqnbv.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2nkokwxye.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2yvocpxnr.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2iaiqbbnb.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2vvmttxqf.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2qjunizjr.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2nkusaypw.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ldebylsy.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ybdeajid.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2anqbogfh.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2iyichvvs.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2puxearie.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2xgemlgew.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2qnhcxksq.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2bmkfnouo.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2vucstsqq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2cehadddj.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2tdsohcpn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ykdlbeuj.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2nonwissg.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jlukoolv.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2wyyykgee.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2qclcwfwl.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2eyihesnq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mraawzft.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ybqrbyjj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2ftsibxzp.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2vtftkosw.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fimrrnco.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2trjsvnay.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2qpntnxrf.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2xlackvps.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ksryoijd.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2tcggplmo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2xbiuohlo.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2rinyknzk.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ydwhxcne.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2qqnvkuez.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2mupukccu.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2osykhwyb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2pcsjexqi.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ytstlyqr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2oebxdpzf.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2sshtbvuw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ojdwsigb.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2pmnlkioy.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2skaabhkc.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ceibkqwv.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2mudgiylu.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2uunuytll.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2uhtuqrce.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2lrgjtlbp.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2dmzpkcog.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2xvdbpkre.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2hpymehvk.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2iigzhptm.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2ditpcsgr.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2dqlcoxkq.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2tedqpstj.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ugbcgxch.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2etzlnysy.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2pmpxbusd.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2yfofltpp.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2elqlmjop.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2azjyblam.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ktdkmuut.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2grrdbibh.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2eyxxskcb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2jwqntodg.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ncipkazl.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2vwndkqmr.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2tvlyfyjn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tadhctmd.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2lmasbdsd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2tpqkpvon.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2asiivwae.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2pvrmdmkc.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2hihbcfxs.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2leepmcxj.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2ckiwkpqb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ybagesxx.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2xvlqvdiu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2nwhdigtk.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2aypctrgj.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2symzzxfc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tdxrlehc.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2hslvkhkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xzsbjgdo.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2btubqyow.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2kwauisrp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2lgiffzpy.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2vzlbyvmw.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ieewrowd.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2hffsoppy.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2obiximiw.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2zgnjzqyv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2xcnjmfwb.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ufkrmgds.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fmwzxgud.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bvlhgiir.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2irfdeqae.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2jowpmaqr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2gtgjbnmz.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2xszylnhj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2mtzefvqr.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2osbenboo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2gdeuaoyx.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2mjgbgrlj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2tttvtmmq.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xyzcioog.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2icdkmeoy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fxykqiht.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2omfxewkv.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2kiuguvvu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xcbnapnf.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2nrxonxpn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2lgeiqkwg.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qdamngox.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2hppbyexf.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2eoqyzegw.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2twnonjul.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2uvtwfozc.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dejhbdgr.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pipminwu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2hrhhpbin.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2sxylesne.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2xsnkxvky.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2eisqadwl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2eownkepq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ssvvaeed.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2trnxzbly.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2qiwfhfsc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ureaokck.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2glbcecow.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2dadvsmxz.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2edusghqv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2bdsrsimn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2unexwlac.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2etmpkpdd.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2mjsftfrl.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2rhxrkvlu.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2dqlfxfqz.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2gicqewjs.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2yaqiheti.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ycgkkeqq.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2kanhalsp.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2flyalvhz.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2aluvkxdv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2fjtvomhq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2utoiveow.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2pfbchpza.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ongsytof.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2elvnjgdt.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xqhucckb.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2eggvnndx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjlajoho.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2scumbvvv.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2vzroxedy.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2tbbuzbhx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ottszanc.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2tlrnqskx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2tocwiemk.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2mqdncnrv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sdxujqkk.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2jzthwtlx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qqpnfhsf.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2tbpabkdk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ytuoncxt.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2ukzhvibj.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ddhualso.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2cnvikmld.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2biugpucy.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2rtmhccbl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2jrphitzv.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2oqbympnm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ooxycvtk.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2wvkfvspz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2rsdxplxu.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ronpwqft.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2pbcuzazm.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2hqmpxclz.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhhauxuw.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ielzqvdx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2zhpxxrxo.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2tjtjoaji.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhgysscx.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fvxjjush.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdlbjhaw.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qmgwwgmt.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2gmprjrka.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2cuyhjjxq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2dmtatbqc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ebdnpjyo.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2gldidkxe.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gvlbfmuz.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2qeeykxfm.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2vofctyhn.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2miszsyvt.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyvbabpj.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2oywpywsk.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2ddeoatfg.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2dsniqwdi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2pblumtms.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2jbwtuvbw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2inxpjigf.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ozptoiba.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzmvfyvl.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2idvaiycp.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2knbcfeox.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2hwuivdwp.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rnlsrttr.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2wmzaipvn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2dicyptyc.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2utwwonaa.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2fflartub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2okazgsuv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2zrkbblna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mhoxekrm.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vqojnubr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lsxlsquw.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2uddlhmuv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2oiqadaci.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2hhbiiblo.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2nkuvbkpo.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2llrqrqfq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2eurgygfi.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ekvpzrdj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ekzkcyxr.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2tqxqhvja.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tldthfsq.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2uhpgqota.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2mhklblqa.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2tluqkkdi.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ypnnbdap.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2izercxzc.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2xgpjycdo.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2tjsbihlf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2btpxnqqr.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2uhgyuziy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2lpamuagq.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2jtopmvea.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2txmkxeil.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2yutaytrm.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qcsvxxnu.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2crdobcdo.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2vmslqpby.html


<!-- 参考信息 -->