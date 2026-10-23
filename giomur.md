代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jevaoili.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3jxcaockw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bcdcagoa.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3usxctnsi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pzsxzeiw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3mvtvmfso.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3qrexuogo.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3rfciudcn.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3lkirvdkq.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zkpzsifr.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3edddmaqn.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3bxgsqtvo.html

esac
来源：http://www.52xcode.cn/Article/details/gt3sfhxmjde.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3rjzqdosb.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3usnjekfg.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3vpvebkad.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yprpymaf.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ojiseepm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3hokyqftv.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fuesdabe.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xsjltflh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3bcohrtbt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vsdceajj.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3uoqbncfm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3btjslhpu.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3heblnerb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3sybbdjik.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3nxwbuqpw.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3sxuyskqz.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3lwgwdybe.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3dkzxnibz.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qeaifcjo.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3jejizdap.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3cjvkqjxc.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3cmtpedcr.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3jlwnqdyr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3qavybhpc.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qlexjjfx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ldfgmfxw.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ywirxoeq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3wvdoqijj.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3vxqcxjmw.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3abeqhnrr.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3uyfuwodt.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3vrjjetpf.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3gtftrxbk.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3dxjyhlue.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3mpmzqhzd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3xvlqjcnv.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ygfhvfpq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ydjkqqbw.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3ipbgudll.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndesowvh.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3rnosknvr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tyyzciar.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3qdhyzmcv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3tzaxwmul.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3dgbxbait.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3lrdragff.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3gawulhfs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3nwgkdxvy.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3pfljkjiy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3rmsbpxyl.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3apvofqtx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3zunnulvg.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3mpuwbjbf.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3gjqvrcbl.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3kogguvpt.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3pbqpiuts.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3gkobeywn.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3rebfwhho.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3hqqrqsns.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3arxoqwtg.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3urrjzehl.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3oeezltfg.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ohklyjqd.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3wehalewx.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3mvlqrtuo.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3wqyqjirw.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3ltjcoraw.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3djplkazx.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3tqxcpsqh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3wotbbdhx.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3uvrmrshw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rlhsfesx.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3emwlqyqf.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3nwvfhxuy.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3duhfhpyl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3sxtklezy.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3rtuppvuq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wprlldao.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3bntjzxew.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3cguywphf.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3tsggsyni.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cvdwnwgc.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3yzedbcoy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3qbptnssm.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3bvpnrygn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3eptbhsdt.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3yirnfwpf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ajonwwez.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wyrvcdts.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3hfswlxnm.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3fxlxmzer.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3aigkdmrs.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3knqdlxgo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3xojafzqi.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3vlclouwy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3kamnunld.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xptmakzp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3tblurgng.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3axwvxdfy.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3kbgovpal.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3itcnhuul.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3jfgruwkf.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3mbdbyuzr.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3pszstggw.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3glnclgyx.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3dkyqywup.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3cmhuffid.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ixkfsxfv.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3odeijbhs.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3dxczylgg.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3hdlizldt.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3bvhmydjj.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3pconivnm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pnbpvbkh.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3ucnhjhcr.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3etqinxqu.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3nojatbjl.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3tqxkxnoz.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jvlbekeb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3sjjibfnj.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3bsytxuez.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3lquhqwak.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3dweceadb.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3syawlqoa.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3yjdadduz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3uccolbgr.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3iivyhrmj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3xwfushue.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3snehquyr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qdficshv.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3kvynupfa.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3edggwlwi.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3olmneucc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3dpfhkgux.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3boouugqc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3gshbkiax.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3tqodxfef.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3aycuttpt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zaatgjlh.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3dxdqtkpy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tuyzlsaw.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jlukabdm.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3ilxmiiyy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3jkmbnxla.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3zmgmnyvi.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3mrgzwxna.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3bovikocc.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3fcovvgrn.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3penwmsma.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3qulmyohy.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3gvihzmbm.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3zqonjuzk.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3plfvejaa.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3xxpjspkw.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3hqjivjfs.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3fraktqpf.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3elnetltc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3evkvsfys.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ripamndx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3hnjsipyd.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3bxambkli.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3rnasgwep.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gbzbpwxx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3vbmvefnj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3yxqloaqt.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qtbaafhc.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3dbeggtcb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3rjulkzwd.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3pkemnvzy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3hbdeiang.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3hqtaokqn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3gedeopue.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3dmhbhhuj.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3pgjflxwz.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3rjcxttbu.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xjigwnmc.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kcesvpgk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3qruxsbob.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3qtratzda.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3pzbswpfl.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3xkarskgo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ckmwufgx.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3wwhbivln.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3uudevopl.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3rszgwayf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ijmgccva.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3kruyeaqe.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3kdtxvcfw.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3lwdlnezy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3hapmtumh.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3zcxtyinj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3hgctbzgg.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3qrrwzrhl.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3vwalzlje.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3dcqwjkam.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3fiwijdic.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3sjykctfg.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3djkrbbsn.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3hrohkkoq.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3fttqvruo.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3aovvnofh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3xdaevhqe.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3iyrbzmtl.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3thwmtpim.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3qhwtqvuw.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3emwnltog.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3txupgmrm.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3rvmdiumw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwynismx.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3adappxjp.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3oxwvggfz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3hfwiveih.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3fskbieqf.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3bnurpaqk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3zzwgrwln.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3vfmjlbvw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3sklmxsrf.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3pjykhouk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3huznhzej.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3prxzrlck.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3hmejaegz.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3jspangjy.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3delrfqxt.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3pimsutre.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3giohdjms.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3jzuniljm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3tvefrrcc.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ngvythgn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3axvfbaij.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3zbdfcxli.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3roduzsvx.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3njzebvhw.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3lpbpbafr.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3dfgazkrg.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3amidxczm.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3iymenmhd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3sdciyvcq.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3fswdfcwl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3wfunulqf.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3tkutdzzb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3bolkvnlk.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cqchxveu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3dawqenqi.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3pfmahben.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3fedxhhhs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3hsokuqxd.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3lbfajhdw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3aovomavs.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3uyvwpwoi.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3ptlzdbfn.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3bjqedamh.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3qyekxltp.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3pkczimpi.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3tshhzbdk.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3catgknjz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ptixhuqt.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3hempvzmr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vwjlqhbt.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3cojuixdu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3dwkpfudy.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3cnipzptf.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3xttlympr.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3yustzddy.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3kwprnofr.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3zuengwdg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3scgrlhih.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3hrdtvpuk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3zacylvil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sgdhanmw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3wffavmtt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3axsjnafn.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fobqddoc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dcjhcgzo.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3clkpeeoz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3jkcoiyob.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3uimjtlgt.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3wjzreail.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ckygvixu.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3hxsupoeb.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3nntspara.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3dtuvgiin.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3urrejuew.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kmqcabbh.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3xmqfkcnv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3sakuwlhg.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3asffmquf.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3bioyurpa.html


<!-- 参考信息 -->