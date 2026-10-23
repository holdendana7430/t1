代发 wailian999

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3riwultgt.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3fhilqpni.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3kxjibzck.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3odtgahnc.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3sdscgase.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3yebmwpoe.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3weroafgf.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3xigjskmz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3wdqxnktv.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3hikogrjp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3uycbvidj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3xndetkac.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gogwbbbz.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3lwartpcd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3apliniya.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3fqiawvvb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dildvjim.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3wqwgcfis.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3kmkvplzb.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3abwdhzva.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3xfkvqgze.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3zelmrpiq.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3cfwuayvx.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3eatljxso.html

esac
来源：http://www.52xcode.cn/Article/details/gt3cpuymnmf.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3hhrtbtbj.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3kxzchgez.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3hrmumsec.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3watnfrdq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3exdmllvz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pugsmmva.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rvwgiguh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3rrjvcakd.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3gwcxbrvi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3nqnbyiga.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3aboasdzn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3nkfczoqo.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3syirroem.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rwsaavbe.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ycsyitck.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3lynrikel.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3vrlqhmhx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3zqagplzv.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3baakncml.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3qdjimtop.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3omgwlyjo.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3cbddbehm.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3iihnjpen.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3pmwrfrqc.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3lhuglvkn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3vqrwvlyd.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3cyzuegky.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3lhjgjaxd.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3gcplmprz.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3eujrqnzf.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3neovbafs.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3gxjpxupt.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3kqeohrtm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3ggfhhmhk.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3fptiwsmc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ekkebnus.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3yztjrxxb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3mtrbojcw.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3axjksdij.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3shgpgmkw.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3wlblkabp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3dktmvoqz.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3xdnfqanf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3wkqmrjob.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3jyvllsrw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3zybgwqvg.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3mmmjwtrj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3nutalhyt.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3opryibbp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3rurdmqxa.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3xbrmachb.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3dohletyx.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3jicdulvp.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ygzwuily.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3qfyubkpz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3qwrslkud.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3mpfbbeig.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3csqpfivj.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ulxivqca.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ssmnhmxg.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3ppchpypp.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jccivgvv.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3xttounyy.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gxnrgqvj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3elzjdofr.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3jpudrkii.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3lvkezlrl.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3gqnhutms.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3tshatjpc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3bprgbfzx.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3gppawkhd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3urqldjcu.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3fuszfihb.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3haewnezu.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3remoufdg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3uguztlgl.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3cupinfcb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hggzvjij.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3xqwrzwgb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3tkuixmny.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3qhkuacab.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3fyjxbfxf.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3uugsflvg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3fdbuulco.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3fjtbaiio.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cmiernnd.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3plvqvvqu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3eqkvxewv.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ehozerev.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3xiwvxfga.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3hgarhzow.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3nfnvxmqd.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3koouksge.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ekuvidur.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ojduqxds.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3vvdlzmjt.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3bganxrbq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3tcikkkyy.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3gfsznwna.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3fljmmdrs.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3yvinswxj.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3mgqnmyco.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ngaeqinv.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ohtkuadq.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3tvhedxof.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3vohngpsp.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3clxszaqv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3oefmqelc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3feshsjbf.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3mfixtefv.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3bibsmalm.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3aoehflwe.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3tkfirgem.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kuwzuuks.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3acoodgiz.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3nddhtnmg.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3xrsuarny.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3thljyvpo.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3kazkzulu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3dpppuhwj.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3njoxtsbx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3hjaazypa.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ngquhujp.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3cfaobltq.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3dcwsaaug.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zmuxeujt.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hdzphzmp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3tsgvzkgl.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3lmroqxkf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qaxikavk.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3bzgjwzbb.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3grdlqkbg.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3uvvdapkp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3wmvkfzlk.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3enzggbro.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3mwabukkk.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ngydhqxt.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3huwnfhky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3twjlmhlw.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3buunixes.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pxucxrsf.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qmxbaieo.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3vksdkswz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3zczrulcb.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ufmygeli.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3jkyfcfut.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3czytuhes.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3qhdkbjmt.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3lcehmoif.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3cfddtdhf.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3fvjijzgv.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3svuklqsa.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pqxavasa.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3poaxiavl.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3afcspbpp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3pblfkxea.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3oteyrloe.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3eeoimftz.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3szxfbqlf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3htqfjodo.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3jfbvinkj.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3bvxwtmyw.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dhybqqui.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3jhpnotot.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kbzikigz.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3oazogacs.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3oarjnvln.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3zulwrjhp.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3txxfwtqi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3llnmghzi.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3bjgiesvt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3jnciyevg.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3kzeqtepa.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3kpjticqt.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3pukincqn.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3xbmkobzk.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3lfhnluuf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3zhwgreip.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3kiafzkaa.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3jpewhart.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ldcubhvp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zdiwejlt.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3xewjhiaz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jkjzkqnz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3hynimwsz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3hewmyfhm.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3raidhkdk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3vbeshzcs.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3fqymgfbx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3xsevlaag.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3wvipmwti.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3svfyahkd.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3pwjucmsx.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3jlmzoqsh.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3bownrdtg.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3quuqqswl.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3tdbfeenf.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ejhykqml.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3zunsxmxp.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3onxdmqnd.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3odcnujkg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3wbadppnj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3vuznxxvm.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zsikbiir.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3hgyhlqay.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3tabqavgt.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zzvjbosz.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3csznqbqb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvykildp.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uljmfxgx.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3fhlrgyjb.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3zdupvpnb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3prfmpsvu.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3wxpmmflu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3moghhvcj.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3dnbzrusq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3csdavooi.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3mggwxchu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3eikwlztv.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ddtapdey.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3wurxjfub.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3aldokclf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3famjreii.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3frtjyqbq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3nersdfpg.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3cggkowgv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bkwpttuj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wasexkin.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3osbawcuz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3tlqzkhwi.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3feukrfjf.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3unhvhhqb.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3jygwxaqe.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ykoqhmxs.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3iphxwynx.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3uembmstb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3jhlzvmsb.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3uubdspje.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3potflbsm.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3unsmyvzw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpblbciz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ivhqiecc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3jsbcvzhl.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3indcffvp.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qfzbvsys.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3jwiaidgh.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3jzpqnwku.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3juehxstx.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3zcfcuiim.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3yatiqics.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ryexzgun.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3jelcesql.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3svieohyv.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3wkenkqhh.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3kghjnvgf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3wgyjoiug.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ossbvinh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3tphphqrg.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3kvxsuvqs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3gymdijer.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3hkocirkl.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lsktbvlv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3rhptifak.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jxjhxhdk.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3mexqyaks.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ndpcamax.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3phbuhsfd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3sbfqvvqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3poydbvcb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3jkyiwgnd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jyurskic.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hifzsyjb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ifbvqrft.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3rstgrzld.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3fkqtkgnq.html


<!-- 参考信息 -->