代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3etdamdxg.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3gtrslatg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3tlruodcf.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3hebbedoq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3qdoyrhni.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3qmgbsrdr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xhfejviq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3svqnjawo.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3comjbwth.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3gedicsin.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3sjeqvitj.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3nzvwcsxy.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3aiwvpnnk.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3afntijdt.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3bxpbqsur.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3zzromlpm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3wqfrslpu.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ipjvjhrd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3qcrxvmzc.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3yegnmqxn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3sqaksqnd.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3rcyoqkeu.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3qmadtnrl.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3oarovzys.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3hhwhtmps.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3byybbigv.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3tmsmwztt.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3vrlmfeyf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3zcnlwgdj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3nufgewam.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3qxkhwlyv.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ovdhvbec.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3qupymipx.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ncmkdcbg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3hdswvmis.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3blvdhdcz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3amuiwyhj.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3xttedivv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3didoowmv.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3phdjmyui.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3oioovhpd.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3qoqkfqhx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3bmqtuqpr.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3fgcpfrtw.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3yboppknp.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3wqydoloc.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ugwvlede.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3wmzfqvoy.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3hayyldgo.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3isnhhtrt.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3fskwonwo.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3pjkbfief.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3yxjdzdpl.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3cdrwwymf.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3idaettwr.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3xfiwnkhf.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3vwfeuose.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ujlrfvpa.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3hmvtajna.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3ibgwslka.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3blxuaohd.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3vmgvsiwg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3rwfwlsvb.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3bbmlflim.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hfuhemmp.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3swnskkbt.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qwllmxop.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3toachsfv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3xrhkxsek.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3tdpkmbpm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wkapmuov.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3caomiuca.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ifthhdin.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3zhlphduy.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3azluztjp.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3difyyewn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3xdelmibr.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ljwdmecd.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tudfesdc.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3sdyjlclv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3xozsmkec.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3rgofqvwr.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3txhdifsp.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3hymkjldy.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3qsztzcur.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3pdddcccr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3envruhez.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3opwapvqp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3nejiweqy.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qvlmjmka.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3wvfjnxdr.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3lzuhvrtm.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3orzruuaq.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3kwcblymj.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ovyqsktp.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3hbxxjlmj.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3flnuolsu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3vrzptefd.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3edzwetwz.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3xqxkunxx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3dtuvbgkg.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3jpaohizm.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3lmsnvvfa.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3mikkekof.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3kbbdclkb.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3evagkhea.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ohndrcue.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3obfclddo.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3bnvnyxas.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3uosxvqiv.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3qgqyspju.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3begeunpw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3rcsbvoew.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3pvnwtwhj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3sorobucb.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3pykxadfb.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3qkkwblax.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3orkxmlco.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vlmitfla.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3inqfivoz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ggsgmfvm.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ybtwejpe.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3zcaeohjp.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ueghnzth.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3icdlmuid.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3dtacidau.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3vxfdtpcs.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3hpmyrgxy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3tmxclixm.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3kkjlajyi.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3afuuwrog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wcdkncea.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3jgumimwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xsunezcu.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nlhdmzqd.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3qtwqlxjb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlstqsdh.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3wygvndug.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3stpnujbq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3mqbbbylf.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3cudldiqe.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3wnhvsfim.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bubtxkzg.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3awkzorzq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vnbwolkt.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3qjrnwsew.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3nbmkejwu.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3wjyzrkix.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3hegbuogm.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ciuaedsy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3qonffrcr.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3dhnnqefs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ojzswjlp.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3sbqrnxwq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ecwuqeip.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tqkqbfya.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3rluvwrrp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3hpujmdqv.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3cbgtkdan.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3jfyxxjqo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ocugatgc.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3iwbtfzsz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3umcxhenp.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3plbafiit.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ihlxeocm.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3gpmsdesi.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3vqqktuce.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3jkqdpckz.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3umvwaois.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rbzlgshi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ajjhmign.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3gfaixpon.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3sfxvjwcv.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3lptxopel.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3wkiyfmdn.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3uvucumgc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3tznbhrnf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3neeuchwq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3daihfhrf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3xgrizvzs.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ftsrlrfv.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3yuqywtxh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3qlavekuh.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3lpvkimnf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3jgsfmceg.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qqygabez.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3smppjvgg.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3pltrdsxe.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ytojylil.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3fzlllcsf.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wzqxmpss.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3rvefpocd.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3nwflahdm.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3fhjhsixw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3unkzxdrq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3feipusbg.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3rcrakbrm.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3mophcmpb.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3yyxftbrg.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mirefsmy.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3klurwwsg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rolhcguu.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3usnvqbmb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3nnzjclbr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3tjquohdj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ditfqcbc.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3zzchmmsr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ngdeuxxt.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3trcotgku.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zlfnokgs.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3johrwjpg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dnoymlhz.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3wcczeaiy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3isucxbqf.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3wkorouvp.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ynvswkbi.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3mnfmlhof.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3tpazneet.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3lmfvobkd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3fdoyvmae.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ttysepds.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3orjjsotv.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ilktfbmk.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3ynrqnfbf.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3zxjwjesx.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3pnpdumhy.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3fanlpfqf.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3diqmgqqt.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3lbtrdysc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3lnzesgml.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3wsfrjbnu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcpmjtks.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3dmmglvzq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3jshhaovy.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3uancvwoo.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3apsgvqnn.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vvigymfj.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3wgfjuitn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3oscncnjb.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3uejpussb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lmwavugx.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3azfmbacc.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3vjjaoemj.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3wsrjqkqq.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvzepajk.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3zaayqqou.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3wvjmpanz.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3pwjpuget.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3dedtwtqo.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3omholnjb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nquuxezf.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3bhgpznqq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3snrohmxe.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3dcttbgcz.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wmamwewl.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3itubxcnh.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ovevowve.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3rhzpuzqi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3birfbgzd.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3oaurfhtg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3fjmvldsp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xupbatdt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ifvwedhg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bgthdedo.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3iswywktb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bionrhyr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3gpobsyvn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3uaoxywls.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ubjunptc.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3iueakgwh.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3bmcakkfn.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3swzafjgu.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3glizhowy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3wlyfiork.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3igtivzha.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dqvqflkd.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tferyqqe.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3sjbdfkit.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3fjbabcks.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3cxhkwpnu.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3sdrganpg.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3nnfldwaj.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3brtojoax.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3efwyrrgf.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3ninqtqkf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3yvllmgfa.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3wicxhpep.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wpkmjksv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3jtamvtom.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3mmauabtn.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3pgycwvfm.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3svzuknbo.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ubaipihq.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3yyqtzuuh.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pcxhmmbm.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3aurtlamn.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ywxjcwtc.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3awxdrwva.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3olpttndb.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3sjcqudsn.html


<!-- 参考信息 -->