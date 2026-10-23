代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3xygpcdyg.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sbuhieqv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3twtpulye.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3jiwifyix.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3tuarlgsz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3yrzqofpw.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3yfzngzns.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ygplkfqb.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3uihrzbzi.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ptkplbvz.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jbomnfah.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3xkflyaju.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3zbzputiq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3uqprjjre.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wymtaojq.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3eydlfclj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ocbjwzni.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3amjpqxxb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3rhseprpy.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3thcqpoul.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3vzzdndko.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3kgvcyhov.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3xvzjnmpm.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3cwiuiqlb.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ybvdyisu.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3kvhkvcxb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3vqbfsmab.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3hxdahean.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ngglrxdt.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3hnyiektd.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3cvrllbcf.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3quexebcc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3wbwxcozj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3busuvsfw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3shrwxjfr.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3qwiyywin.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3watypcxc.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3rcttorhj.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3nqmrygzb.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3eaokywsa.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3qvfskwoq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3ltvdkkyf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3nlyndcdd.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3jxtlzqnr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3xyvahdoi.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3sxyyubrg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3shpucoro.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3kjgmbota.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojonvwga.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3gqlyeyoe.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzhywtvb.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3hwyloqdp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3npmxmjgv.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ctqdaxet.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3dbgainat.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3phxajzyw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3srunkghd.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3oilahsfi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3glhaatws.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3xklvjoua.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3hljbkxle.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3mgoxknkz.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3jggovvjt.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3mikijogu.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3jlevwjyi.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3zetwstxj.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3wtwgbcsw.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3wlrkjfqa.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3czeofydm.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3sfponvcr.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3pakmizcp.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3hzpsrsyt.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3jplistqe.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3bzusqwen.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3vdsbgcfm.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3xcmfwyvz.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3vwxzbans.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3zopyfysk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3gijbzklo.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3bwfgwuao.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jpgziqep.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3gvqozmgb.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3amcxbvfg.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3xuedilil.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3updjylpg.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3kzezfiyj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3magsnbvb.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3moypkbao.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3olkwqzih.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3zclijgdl.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3xtrdpyyv.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3oxngvnib.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3rwepiltx.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3riaegraj.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3gnosdnbb.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3jnaribfl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3afuscdow.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3kbuyhlww.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ybbtyysj.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3vefppzpv.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3lejrhvpu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3zhbwtrpq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3mzxilcxf.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3kckgraaa.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3qtmgbfay.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3fvqgutyy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3gxupwfkk.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3kouvvtll.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3eruvwfkz.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3vqlnczyj.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ckkrucar.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3sapcfled.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3khitmyso.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3vuttdvfw.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3bglliiuv.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3kirxcjwd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3yhmkhjku.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3gljzphdh.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3nbivttht.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3vjlvnmnr.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3dhiksuqd.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3zgsdkfga.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ogeewume.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3wzveytff.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3xhmhkgbx.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3lmqdgrtb.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3aomvohsh.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qpategun.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3kspqtxgs.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3jklzskiq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3vivnelcr.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3higcohyg.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ddmskydv.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3egyerhzj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3taiqcvbp.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ynjvnbrb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3kbbzufqm.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3wtzhjgnu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mxkionce.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3oawyuzri.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3wvumnknw.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3oymgbktz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3bzyrihaj.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3hialppxt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3zjanzerz.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3zbcoflye.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3dinyrorh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fiuizhpe.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ivqztkda.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ggbutfad.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zwziewjp.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3qnjmaebb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3goatqulp.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3bmcalhju.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3ustrnoqf.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3wejmfbfh.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3neeqvlkz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3aceqwhft.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3kwwozfkm.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3bemcmddx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3svdotdkw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xmqrumwh.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3uanhoyow.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3hzabsuvl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3qlqntgfe.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3bswjlxip.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3vfwyzaoc.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ztgagrqe.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3zhxytfei.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3gdapeoyl.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3dabzxyuv.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vgznznmv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3cifmbkab.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mywdmcpp.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3cdkkkico.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3tpetjfmt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qppznuyp.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3egkmazpw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3eouskhkk.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3sxykoxct.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3zsbhwiig.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3tbtymkqq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3wzhwsilv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3qycksuhz.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3hvzkcsvm.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3unlswjjy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3afdhydhi.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3odrqpdml.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3qmwejryo.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3hgsimqsg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3mvjztrdu.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3luapaiqa.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3boofsqft.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3xagyygtb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3hebwhjfc.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3gismfpil.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3qkyycesw.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3dbydtbfx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3kpohezto.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3rjrlchoe.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3dmlakxcz.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3mpfkttvs.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3vopxjjjt.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3tyrysqty.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3vlaqlnad.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3srwdpvtu.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3oyviwhfr.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3zdjjsbgq.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3mfwpsdcr.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3enhakvho.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3jdnfcwjz.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3veiiofqi.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3xmhytzzg.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3hjmpmebp.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3zggfhixf.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pzxiymhn.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3jlvdtztb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tykmderv.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3oyjbqvos.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3hhseukqw.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3wzdyotjk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3myscdpio.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ztxcuqmp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofjxivsz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ojjzgvkc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fkmiwgxj.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ubszrwmb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xxuxvoxg.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3lywhxedi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3sgqappqy.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3iorjhrln.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3rwbvvntt.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3hpliuimb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ssyjiyns.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3clirxzfo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3qgserkug.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dspiaflw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3adrggknh.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3kbtdmadt.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3bwssjjmj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3eznwydag.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3emloxfec.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3vitazdlj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnszeueo.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3nuxjkuoa.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ahsqbrvt.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3vbcvkcdv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmaemrzn.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3auvyrbph.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3aafibgbl.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dsrfflxh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3awkxghlw.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3cylrqxjl.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3hnittsao.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3pacigjyl.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3cwgjmckh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zefchwfg.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3iofnpvfy.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3aapydnjz.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3vunhqudc.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3cabpakyr.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3ammzuayz.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ibhzbmyg.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3kdfcamvj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ulsajbba.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3diexpkcn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mksalpga.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3lzfeqanj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3wbsnzggy.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ohitocyi.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3blpbkmqy.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3azgurvtb.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3fqymctxw.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3emfmifri.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3xhilpajt.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3drgqkphi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3qqqhcblp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3obnonxvy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3twpcmqjl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jxnxfkkc.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jagxtyqz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3neqggrkj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3rmosphnx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3uxajtqlu.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3xrngqfoi.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3tqnwagxy.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3iaybckfm.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ruyquiug.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dolpdfqe.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3bpaeuron.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3mtxnmkuz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ldjuufsh.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3mknmvmjj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3jzjllfob.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3lpzwxqta.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3bajjyfsu.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3fykaskff.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3jplafuen.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3uajeidus.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3pbhfgqxn.html


<!-- 参考信息 -->