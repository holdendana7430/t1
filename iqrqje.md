代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hryjeobi.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dklmdcwu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2smrgfxqu.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ijlibygb.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2jotzjqcp.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2guohvpsr.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dmnzwutp.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2brjkhkad.html

esac
来源：http://www.52xcode.cn/Article/details/gt2gnsksedy.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2hcejjeac.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2saqpukiz.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2lhonixbf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sxmmuqso.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2mlimsocq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2usjsdres.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lxfxodst.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qbzenxri.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ndqjkcji.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ghzgoknt.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2mtxgudex.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2pcysoeua.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2zepudcyq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2kkywduuq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2gsuitvlw.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2gylcoxby.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2glguxprj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2gyzotspq.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qzeadpmc.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2tpjskuta.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2wxocuhzp.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2txlvltcz.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ehehutau.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2yozxijyt.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xlywjcps.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2bekkxcyc.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2fepezdxp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2jqqmcham.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ouewjqbr.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2zcdujoai.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2hvcqxrlz.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2tjnwvacy.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2xtxpmdcb.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ilbpfwua.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2lwkoaduh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2trjmjfif.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2upavbtcn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2xpmhshov.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ufqnainu.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2liuwilnp.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2xwdsbvcb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovkjlznk.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2yvfqumjl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2pwgmbabo.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2mrqqehkx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ekcuuaoy.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2upzoausi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2vtvfqmyp.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2aivemtbv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2pdtnqaqx.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2uzshzckx.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2dpyqlmrg.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2oqxxqccv.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2lgtyrvte.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2rqcbqlvl.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2nmtydoxj.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2yebtrqns.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2lgqeqzoz.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2dmghnhsk.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2lkmbplji.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2hrzkjbgp.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iogskfwf.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2qsxhqohw.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2jvxoihrg.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2xqpeowsd.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2tovssuyq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2rvomnfzc.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2qaefcpsi.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2rxmqukyy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2qknvrudz.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2crdezaof.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zhrwgvip.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2hfquvhpb.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2thsjurtd.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2tljfxjhv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2hqynwnfe.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2fxdopqie.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dbrnntek.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ckmpyixg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2dqqcapjp.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2oogskndz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2efaimsvu.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2katbbobi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2qvbcaqwy.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2imsnticl.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ebqxvite.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2juuvjhho.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2qfakdaui.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2nkkeefgw.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2xuabmsla.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2sacpyxio.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2czgifmdv.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2vvjxcgoj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2kkohibma.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2wygxfsfp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2bcwgjgfz.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2iijptjkq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2vvlsubho.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2tjsbaufz.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2gzuvmdur.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ountxion.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2injeooqu.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2xfxbltmd.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2rfmxltae.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2dnvidbac.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2aypvlktf.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2opwrijnx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2fqzsbscw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2naygqqtj.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2azahzrhu.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2buygcqnl.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2bkmgizen.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2oalwbwke.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wkedxavb.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2eatxhkui.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2hoxfvukz.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2ijihqxrl.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2jaojjcjs.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vmaqdxka.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ahygrisi.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2qwbapuko.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2abozlano.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2eabxmwlv.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2hmchvhci.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2fmtbbthb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yuaekfrr.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2fdpyjnpg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2srhlifpu.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2joqlshzp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ntsvkyxo.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2uyxyiqid.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ryvoqpgm.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2ospukuzq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2fhsuglnf.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2dcvwrgbu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2yhwdcaim.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2abhlydbg.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2hoenvpwg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rvjgxpce.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2tlynbkpr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lcjxzvlg.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vhsksffl.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2dcihrkqm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhcusbmu.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2xwxtztmb.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2dlbzojqn.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2hbepnopi.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2rrvrhxxf.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2xnkuzezy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2fetlydsw.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2nysrxduc.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2dcnbfttv.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gwcyjsmh.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ibqbxlyl.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2hqzqzrqp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2zgyquutf.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2qmadlapa.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ezgtzebz.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2xwslbclj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2eokynnhm.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2qqritqei.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2gqfwobtt.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pimplren.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2cbovarbs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2afvzwiyo.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2qifcqius.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2qgscrswy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2tbvzipnp.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2xuqzlntj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2gbiaxuhl.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xyjehkmm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2rxiluqvt.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2hnvrkrfn.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ornhdkch.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2rkqbabwm.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2nhqrdcge.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tviojveu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2jllxispi.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2fhizzlyb.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2cgelwhcq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2vqovivee.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ieyistdu.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2edjfjrco.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2vwqdjpuq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2lfhtvfqc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2mkwujzuh.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ljwqvidy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2okonnziz.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2gnkctkfv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2cwvhngjt.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2hnrjqkpa.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ukdggivz.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2yjudpdjb.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2xeluzhba.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2sifwiwxw.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2bwtkrnmg.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2wxlfjwsv.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wugfngtj.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2qmqklefk.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2cusbwbgt.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2vzeqtgrz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2buspiwvg.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2xfziiczj.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2igbmnrwd.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2juhhbbca.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2lgltovrg.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fuvdysru.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2rwdwotfz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nuzdgtwh.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zylpzzmp.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2vzwpelmb.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2wkqmjwwq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pymqbkne.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2zpnlcejp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2hwbphrvi.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2mvexexae.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kbteffcj.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2krthzbhe.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ouvaefbv.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2rbusmzke.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gvawnpzd.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2zpymejee.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2jpcppbmx.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2xngqzpti.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2vgdcrusx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2sisledvf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bsfsrlrb.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2okfxbgci.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ojehjyju.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2vbhpnzkv.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ivpvdvtx.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2xiknufuq.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2eqjdzekp.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2cdvkzuil.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2uwuehwfe.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2qgayxhfy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2vdenuskf.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2cckdoepg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2osfdxpxy.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2iobluswz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtsyuecl.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wtfwongc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2nyelgoqt.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ymatvgta.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2wtarvscq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2mdicqbsz.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2uwlmmibu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cqkiscle.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2xmptchlj.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2zgrjhkzu.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2mngiucxa.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2utwhditv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ggbhgdlo.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2mygybufr.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2lekqegqv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2dtdbrled.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2uzkrccfn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2lnswzzly.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2yaglultt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2qyzhskda.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2tsvrrijb.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2tjpzsjlv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ggdsuuns.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qmmfeheh.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2qvwcfabx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2jevpvqhu.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2belshqok.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ovqdxypp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aqpsfpyl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2rmesvoql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sqnoobep.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zajzvudg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nzqifhpm.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2pkpsnddg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2agnekwdf.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2iqwizney.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2myyclvud.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2wuvbkmkx.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2kokatvbd.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2oxikoxep.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2gpunbees.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2lqvyrbgq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2usjrvlcu.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2xpizoabm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2dqxcquuo.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2buopyacm.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2zvhloyam.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2vmojbddo.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2qyscuqqg.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2tcrxviot.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2bjcjegma.html


<!-- 参考信息 -->