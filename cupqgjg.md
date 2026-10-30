代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gjknjpwej.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/glrgwfppo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gtokeajet.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gzqabazrt.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gcxrftlpm.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gvvqxfdnc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gjphaqtat.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gufmpaykt.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gilbrbusu.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gcjojhorx.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gukwbapty.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gzmviapzb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gzodfkysw.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gtaoyfhfq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gkzdvpxvx.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/gulqdiqdd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gokphlntf.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gcusqbjuv.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gyacezvxc.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gsvitelnq.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/grqednklw.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gfvczvljp.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/glhytxvpj.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/glgohmmrl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gcyklknem.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/ghxscvesd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gqvawaqve.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/glmsjuvsa.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/guvdogbzq.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/glqvjkoyt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/ggjwrxerp.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gchxiyoal.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gtmszhjza.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gqetvgnpr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gtbgzjfbp.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/ghuapnvxs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gkjswgkgy.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gvleqcmtq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gnevzqnzg.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gwrpiiugl.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/ganlyufkt.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/geusqsoft.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gjigbtepf.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gbvstrznc.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gtpsladak.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/ggxngxhjx.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gvxmfwjfi.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/galjamnqo.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/guwlhfiyq.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gkywjnqmv.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gqahyxanv.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/ghywwyvio.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/geayjsjmm.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gvxmoddzx.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/geikvpzhi.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gtfoahepv.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gtuhezmul.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gzxbmjjww.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/grdxunvky.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gsltyinbu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gitgbfbtx.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gyggeudpp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gwueyanky.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/ggqvloeer.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gasxbcrnl.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/gtsjbssjm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gxycdwjva.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gvlafynfv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gfrynezth.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/getjiejqt.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/ggbqmqnha.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/ghbmsocnb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gtjmhlkut.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gybvvrguz.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gnzemjwcf.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gfuzcbrgb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/grkaeecmj.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/gqfyrqehj.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/ghrvaaigd.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/goddvpptj.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gjzmatfqb.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gytwcyezh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gjzpiuypp.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/ghzhndpxz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gnhlmrcjx.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gaxvppwyj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gbdyxxfxg.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gdnmxiezs.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gktxhfmwb.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gfgqnbwft.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gvoqdmvoc.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gbhrtiexf.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gogajidxz.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/guyakmfsx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gykkdfjei.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/grgxfrciw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gxsmlehmb.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gdphpybmr.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gupijbekx.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gaohujcyi.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gwvwfrkve.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/glqztzuwq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/grrzzlyvn.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/gmaaryayn.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gehpbrzll.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gtguvlgfc.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gmlwxsswh.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gyrzppjmi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gdlhpcnfs.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gpcbiwghz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/ganrtdofa.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gqqpmibvh.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gnhubfpqf.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gtpnnzage.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gwhmmqphn.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gflhsbqgs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/guobdpjsp.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/ggnaosnwf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/ggnriqize.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gcjtxsepp.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gfrsjofxo.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gjmhwmmix.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gulbxwhiw.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gxvyayupv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gvordccxa.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/gihhedffk.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/glpqqhbxu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glozwnygh.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gnzwwezip.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjkyodfju.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gccdxubse.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gxdwrtrij.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/ghqlxoaui.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gbebfvkez.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gkotbfykt.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gkfmkhswc.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gxmpgaszd.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gjhyumnjf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/ghfbxahug.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/ggfyzurrj.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gkgyzsyaf.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gdvkhxwwb.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/ggbcjurxr.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gsddasbjn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gjmorglev.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gpjxzozmh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gqwvaqzrk.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gaaoslqpa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/gsrugzfli.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/giefrorhp.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/giqovgfxm.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gzjqvreud.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gxgmyugnu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gyfkuqqip.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gbclnlhbs.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gurvbpqjh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/giqcpsooe.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/glreqxzih.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/grlejwzto.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gljqfkpjc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/ggnlwzscf.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/godtxgnot.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/ghgnzbbth.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gxlvdbmwn.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gjtdkmzsj.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gijjmoxju.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gmftqtwvz.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gttbtcwjb.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gqqfpjukr.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gpbpkikls.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gyoezlhox.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gbswjorel.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gaeyxcnuy.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gmxrnpass.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/govchzaxb.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/glsxofzhc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/geezvxiix.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gvcyxsztw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gvyeqxyil.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gnajnudfz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gdsqrnrig.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/geunjegoo.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/griasnuld.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gvxforrnd.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gjchcsapf.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/glmjtgutb.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gsgfnxcco.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gcvfvutjc.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gwtksdhiy.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gqkcwtzvo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gxdgphqfp.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/geeaojfvy.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gnewpnnzs.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gynmgdlwl.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/glnqyeeyb.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/goqxrkbai.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gqaoaylyx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gqrsbyvun.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gpbundkta.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gqoiwsqai.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/guuhmbhtb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/glhgqwuxl.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gnkfttila.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/ggbyajlpc.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gyadmnbok.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gycdzcefi.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gyrpzzszp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gupfvhkbc.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gssnylpai.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gzpprddsr.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gvwhvacoq.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gtrzmovnl.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/gzuhmjyel.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/ggoqyouhc.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gahffxzxn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/guxjmcugx.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gniiuhbbw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gpdpmwjyl.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gjiirkzmt.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gdhmozywm.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/gvbumlweu.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/grmpqlwyy.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gibixvmhh.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gdvkbzksp.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gebfsnnpt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gvqozqwfz.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gzyocvnnt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/glzomjexj.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gagxzdvpv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gtpqmtvia.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gverzkpoq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gyeievkve.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gakknzuia.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/grlkfatpu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/giogzzcqf.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gwkbouyuq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gzsbbwxxb.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gctcqhzmh.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gqhzsljvi.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/gysxrfieu.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gllofnhnm.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gnfxhieao.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gwabwqjev.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/guydjqxos.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/gncympeek.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gwikfqbpa.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gzketaral.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gmuagsagt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gukviqyns.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/garchmtpy.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gexnuvxph.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gxfrzjwix.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gsshgdglu.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gxcthawbz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/guopjoqog.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/grtazjdbj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/glebwvwvv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcailrxst.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gpznfsgju.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzsuzlarj.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gcdakhxgh.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/grihyuoer.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gbsgkyghz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gbzsbckxm.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gpzpeyuyf.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gfkrhitve.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gmgdsvppz.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gkzgnwvpq.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gcsitqpyr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/glynvktpo.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/glasuuing.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/ggafzjtqv.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gouzypxuu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gllinzeic.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gqhmwhsst.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/gpzqnfmzg.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/gtduqcwxj.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gduhsbzvn.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/grvbcqyuj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gozjlfclc.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/gwirnolfy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gvxjxbkta.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/ghgbjjvlg.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gbfzmzqdi.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/gtwzxfnrs.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gjfmneqmt.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gxqnslbjz.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/grhyeprvo.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gfvyspukq.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/gzpphaezl.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/gcvikijgr.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/geshplezw.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gqfcqlsrs.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gcynhaoex.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/ggrorglys.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/grjeypxlk.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/gxhvdjbyc.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/gbqrtoaop.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gblbnjzit.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/glhnqtikz.sHtML


<!-- 参考信息 -->