代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ebznyxtx.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3otfsbcrn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3oyobyxqb.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3rsxffcny.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3sbseixuv.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zjwrrobm.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3mniapeoc.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3omvgshzs.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3wzlliawi.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3cdblupkm.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3xrnsuxfs.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3obutedjs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jkvzaggt.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3zfwwhonk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ikqqpjjl.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nibmeskg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3epheflmf.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3snbinpff.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3prpxrrwj.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3oltosxbx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3nxlaptae.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3wwcsozbf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3hhfaxvgt.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ubdynhzl.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ndnjqbyr.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3nbbnjsjk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3fywibmxl.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3novdqdzr.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3zcoqkgnl.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3omosruch.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3wupdvkzn.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3tzotptcr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3apevftal.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ckrzcuvb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3bdxpvwwl.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3gctydshl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3xacmgoyx.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3fqgrgsby.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3dgpkudlg.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3zjvvrvyd.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3qbgxvavf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ajlzkuvi.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3nrikdjna.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3krnqtlhz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3pzuxkeof.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3pyueijpo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3mukeqkfs.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3htwplxel.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqnbpexm.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3tmluvqju.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3uqyqlubw.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3jblbithq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3yykjqhlg.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3olaxrbzi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ftwhwtbo.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3ecxudsbl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3bzoftzhu.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3gaukgxub.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3ztmncuhq.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3bndxqdsh.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3jjiikghp.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3sxxmzmkf.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3fzjydfxs.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3hnsbonkp.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ylrfscmz.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3tbnvwfdy.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3fysyctiq.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3devadyzo.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3hlyrelzb.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3jfdlrbwn.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3zyybqeqs.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3njiejrtt.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3tygdmmss.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3deyanztd.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3fjrijoha.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3toahrjsb.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3xcazzpoe.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3oithmpsm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3atlqqmmt.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3dlohjvdo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3oamfvvky.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3rrkekyjt.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fehgfidm.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3gfkipwln.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3wciawlfk.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3hnaemdbj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gcgcfede.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3wnqwvseg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3lzdxsxsq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3bduildlz.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3jmaqrofy.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3iprytqfd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3agtfvczp.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3sjaopeyd.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rkffqcoy.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3hvxrqcan.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3kbgvsioh.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3iiudmxgs.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3bklnboeb.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3gghtrrbz.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3xxpuuomn.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3qqirelzc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3djcwsekg.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3vheyfqgl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3vczxjfig.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3wayjyfpy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3nchbkrik.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3yagotixu.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ndghczez.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3steejfdj.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3luuamsgd.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3qjwwnpkm.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ppdxucvs.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3hwveowyz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3dneccoie.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3zzevtwlz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3cqmhnfug.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3pguysorb.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3vkbjpqne.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3drcjreid.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3teilktak.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3pewbpojd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3puirrlrw.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3csxbwvvf.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3nvrkhcfd.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3yboplkim.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3pndrxmzi.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3wusnydju.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3hnefffdq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3mdsezdvb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3txtvymag.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3tmwytrwe.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3dcfsdhpy.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ndibndms.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3iqmrgpmq.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3rudprqmr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3kyngzzji.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ngaarwdx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3zshbfiur.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3bphepobl.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3kybspabs.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3uzmqtifx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3essmeeki.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3buzayuuv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ttufvtgb.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3hgdabokg.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3wfekedag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zxjbsajd.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3fnzkinbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vgjqbraw.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lqsywpbq.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3cfgwypzu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkpmdqpb.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3yecgdvyb.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3sdoifkaq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3bxcpkszn.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3swridkiq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3urcespay.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3quklikbn.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3musmkbwx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ontrfaqj.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3lbrwijjo.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3lotngvnv.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ayuktjal.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3qkcomzih.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ppyqqqfi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3nlcpsorb.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3dvpljlys.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3qfxlyyro.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3zowouqms.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3vavxtgyo.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uvwvjbjq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3gkpynymz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3nwzqmcag.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3jknmxpyg.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3eyfsedjk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3blsvnvvu.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3lnrzzkqp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3tjdlcdar.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3zvbbuvtl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3enarufdf.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3waoaleib.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ctlgfsbr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3zwkutojo.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3hsufeoah.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3olnlczrc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ifsvccul.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3dfezgxnj.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3wfomefkl.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3yiurpcuj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ctemybzp.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ogndiryd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3xzeqsjrp.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3kcsebuxb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3fcydjmvg.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3figjhaxa.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3pxrsrmge.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3trhwxuwv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ogaydywn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3xukyvysr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3objgnspb.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3snqbsxid.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3gbmhpyku.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ploaefgq.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ffntghxv.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3xbnrrxrb.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bsrxynve.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ckmeeipf.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3cikkhiol.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3gvnmjysj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3dwcpcnso.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3eyslszam.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3xzfrhpcr.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3txcpvrjp.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3huyjhafb.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sagckiaa.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3vwtfjmsp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3rcpftkio.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kegbiyeg.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3qvdtjcic.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3lltmhknk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3culjmghq.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3iuezjqae.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3kmzogmbz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ilckkicx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nigyulqt.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3uelhnytq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dyeatekm.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3dvmvwvub.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ftygxabg.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3gfchbull.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ydggdxcj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ugbktwtm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3mcbsvymt.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3gfblukdg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zlhjkada.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3aobduvpv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ovohpefq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3lbomfrjv.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3fbrzapaj.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3swhgoqdo.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3avrzxvat.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3rwybqbkw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3xmmnljzg.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ptzrhpyw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3iuznvdll.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3jxsyipee.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3iagtterj.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lwndgsse.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxfkgcjq.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3exuxxhwu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3rwwibgow.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3abqyfjkj.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3dachzgtx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3jdhrsxox.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3bohjdopp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lankzhqh.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3iddxckgx.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3tlmsccew.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3xbpgrsaz.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3mohpsupl.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3nrixivwa.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3uenxyrvc.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3sxbvkphm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3sddwgbyr.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3pznvugcd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3kgwcgxcr.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3gapgjxxw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozaubrrs.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3jfkenudz.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3wvqjytlr.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3nwtpkgaz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3czyyhoyi.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3yguajnso.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3domppwic.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3kmypxuih.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3mpziclug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dhccibsf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3oqqaxzzy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vgtwrvje.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hejvlxic.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3eiiafyvr.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3hehkmchh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ilbqhbdd.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3artknamh.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3tcronlbg.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3urpcurjj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ejnesyjr.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3sjjmmbjm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3wkgiwjcy.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3mtjauckl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3iwizakqm.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3czrjoksm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3loxgcdzx.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3jjzkiavc.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3mqwfgjzi.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3uenbpwbc.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3esjfjfmv.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3zjsiyueo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3icnajiqm.html


<!-- 参考信息 -->