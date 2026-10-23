代发 wailian999

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3nrbgbqek.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3wwstzttm.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3dngdiuzr.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3dtcmyqry.html

esac
来源：http://www.52xcode.cn/Article/details/gt3nvlfamwq.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3hdehohqx.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wzpwyddu.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jaifismu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3bxnofiyr.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3gvikhsgs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3kamcxsxt.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wzinwlja.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zsqklyix.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3wossjmsd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3fjdmhxha.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3fjecizkp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3amihabkt.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3xfqeoqoo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zflybmzc.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ukelcwaq.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3xjajblja.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3mgkyadhj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wqcaxbok.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3frjsofce.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ioloxuhj.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ecnwixol.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3weausgmh.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3piczvmkp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3llxndxjs.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3dnaugeie.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3raipfrko.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3lbjxfqme.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3pjbyyhwz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3nyevuuea.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3yfaextrw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3jrrfvqma.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3karvzquo.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3jjxxdkkd.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3aqpbpvvn.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3uhsulpmt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3bvkrcmvj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3pqcebjqg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3vjulvngm.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ffvgqhex.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxmqvulm.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3pszajgsh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3rnxfepti.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ukrpeast.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3woxczqnw.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3obyvkigt.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3tbtosfft.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3yuvxrtoe.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3ivutpgrc.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3zmtndcko.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3pnhetfll.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3lyjdvlzp.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3reogxpmv.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3xvtvjqur.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3vlxyuptj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3gfcpswpk.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3txcmxpfx.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3dkuxukhf.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3hbaecmnn.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3iqkgtsjq.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3jsjjfsmn.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3bkjqzxrj.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3batnrvsu.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3akktzuvc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ergmwkor.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3bhheijue.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3bstmseiu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3wkbuqgyz.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3bchyabdz.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ovuojrex.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3vclxxrqm.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3rcxomvkq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hsqyehck.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3clpunsex.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3bbxfsvqn.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3frbsadgk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3xdubdmbr.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3omxxmtfa.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dynpyrmw.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3nvoyvsem.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3aguaklbf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3fspreiea.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3pydlmtba.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3xmoirfaq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3hstmnqgq.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3omgvqjry.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3mcrvyvtj.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3qrrffvfi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3qekzkwys.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fnswzjue.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3xznvipkv.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ebwsgotv.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3uihdkyxg.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3lcfvnuho.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3yuiryckj.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3arqaifmw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3qqofpwat.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bliluxgd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3kqtaongs.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3xktvmrtd.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3sabnnuia.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3eetxfyks.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3svibuiug.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3mzixspnl.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3egejfwck.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3sppbykza.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3jhghrnho.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3xpvsryyl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ciltnnxq.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3bdqzkqfz.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3wfzatkhh.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3gnfrvqdm.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3zbnizzoi.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3cbaezgri.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yhlkzxku.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3nsqifupw.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3fjqeclwr.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3pfcwkqro.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3uuzdrwgc.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3wqbtkvgq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3qauqlhke.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3vcfvpetk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3dhlnpzet.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3lygkkesc.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3rutvrixb.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3komnbtkl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gxlzcegp.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3hkasjrwr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3jorxmcjl.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3jvkmpigt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3afiqxnyd.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ficuecdu.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3dyjgqdzu.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3mqdpdjtu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3xgzaflqu.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3gykrluxu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3qogzsndb.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3gububjxc.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3hddnndqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3blycxjgr.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3wcivvsjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kbgureqe.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bujtnbxn.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ougqjotm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3vckbazcl.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3dpqrbwij.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3orvarbld.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3yrshdbba.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ugwflkia.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3geqophye.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ujkccjpg.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qvwredkf.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ejxodusj.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wnqknpnw.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3hmmoaocr.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3qxkyiahg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ilhtdyto.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3upskphoi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3pfkotsms.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3imfxgepx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3wxcowngc.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3wlppsyjl.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3wrotvbjo.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3slzjzpix.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3nqjsjvyi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3hrplears.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3eyfzomui.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3efzwqnwu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mbhpoeno.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3vnmucjjj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3azgfbnkx.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3nnwqphki.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3snamemik.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3vyrsckhw.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3qvesconq.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3bbgkdlrn.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fvctlbna.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nyhkplan.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3arsfrdet.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3qwjzqvxw.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3kiuaonpv.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3lwbzxyzu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ogcdkebk.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3zxlxyxdb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3pmywpktt.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3miwtabzc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3wdjmhorx.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3wbxijjrl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3dqvanuln.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3bgfadbbo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ugxymouv.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3kphhlyfu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3dejbstqi.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3tbiqqkpc.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3lkppngpm.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3pasydilv.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ieryfsvi.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3kgdjwzud.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lgechcdv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3uoxpmiwl.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3mvkdadtc.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3navsmifj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3jkmkrvbe.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3zocvtnnm.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ahlbjhnb.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3bxijpqtm.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3veoopmsv.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ipltsmjp.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3eoioymtj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qotvhghz.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3btfthiui.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3jrppnvhg.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3aufbrfgl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sigiahbg.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ojtlohrq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3lebxfojf.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3mttufdqp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ivmnopvk.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3loksphvy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jnvalqkw.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3fuvjdphb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xorqshtk.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3bxtwqwmg.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3mpbrkpvh.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3vhhezqnq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3pvginfzy.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3bhdqbixt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uvfemvej.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3vumgraws.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3odbhwfks.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3trduwpyx.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3lubejvyl.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3vuiwsvxd.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3mrrqvtjz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3jrrtyqso.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3nyjuhwpc.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3iblqlhil.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3hogiopgr.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3fdouxgmm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ocddhbzj.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3xijnkhni.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3jutbsbsj.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3knowgvlw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3clqcqnps.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yadnddrx.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3upbzjgxv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3cbgbbwkz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3gdmiwfrg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gojjunmf.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3aehwbpui.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3cilxmcxl.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3nwnpwgfp.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhjxwwhm.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3rpkrorss.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3hnsoigxu.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3hzxrbisa.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fsawgexl.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3okdeeeic.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3pjhjtajq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3nmcdhkrx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3njfffdiz.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3ycalnogs.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ckaeoekk.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3mgtaqtox.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3gfrpsqbb.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3sqdpmioo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3kdtgyldt.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3agegnixx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3cxcgqhpf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gnnmaezv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3mzcyrdlc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hhwuosfs.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3corjetgm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3trciracz.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3qvuxerjj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3jetdpcmp.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3xjdkalus.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ifqteagh.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3rkocmnde.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3jjmgmqcw.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3irdfdauf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3xcgigbzk.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vyklzduz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3sdvwvxkb.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ebyxtyrg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3xfrawmcp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3lzoqzrbz.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3tjlndiry.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3nngwdvab.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ogmnomim.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3zmswlxak.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3kzdthvvq.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3zuadwrbn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3qvqcybng.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3efwewwdd.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3olaetnsi.html


<!-- 参考信息 -->