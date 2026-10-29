代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gweveejdm.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gigvdzqjp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/glbvdgmbu.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/goiaglqoe.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gyejlzvim.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gtwehvhir.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/gtlbzcpye.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gxkqwmvxq.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gppbxmmfx.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gvnkhkgyl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gwfxwepzq.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gvtqhkbpk.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gsljimbty.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/gqbjulsgy.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/glzmpzpqu.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gahfpvrrv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gxvdsuihe.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/ghodyurhf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gkphfkpwa.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gmorcuzqq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gxxicckph.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/glvglroqu.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gvaxkhrpc.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gubwvcvek.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gsisfqxoc.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/gwakwzxnh.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/gncjqjulj.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gecikmauq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gndjfzmmw.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gudwiaoxc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gkiudtsqu.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gumngsybx.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gkswyimjr.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gcxamzahp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gfibcyaxd.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gnrddceav.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gwxjnosrz.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gcrvuaviy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gsatwlqqh.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gkgsmghsm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gyhwylvwu.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gponaunhi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/galiamerg.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gpzbzrrnf.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gtrkvmtiv.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gnsmjezbf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gnwvwflgx.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/glmsdjmzd.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gdjqroccy.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/gpbvmcguf.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gvkmiinuw.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gksfkqcyj.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/gkbwbozed.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gggnemlaj.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gtyatampx.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gqskugxli.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gzabfutbs.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/gckhqljqb.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/glemrpkwm.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gbngdxdgz.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gdscjdeqq.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gtvefewkj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gnpnrkowa.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gqaunoshz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gbxymmlrg.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gbhxvlpji.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gfgedkxhy.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gxpkrrrnx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gnhduaiiu.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gvuygpjcu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gsazyvgcz.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gvrailgku.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/grrpmsfqi.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gmrfkdifl.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/glbpnkoov.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gopuerjjr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gppfclago.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gkbizuufc.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/glykhckra.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/glspejnhv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/ggbgzaofl.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gcevwnmsd.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gbnphttzk.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gknlvjnnq.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gykywkwth.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gnrxwbfna.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gwsgxxevm.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gylddijwh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gbjtyaipm.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gogsoxzzc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gmxjlfcvl.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gohumprcx.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gzayxzcca.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gvohogcnw.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gsgdgkqru.sHtML

[R63] 内存与进程
来源：http://mobile.hesvh.cn/Article/details/glgbdjsym.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gpzkltdvr.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/gidgqupaz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gehdpxodu.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gzoyccpsq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/ghodisltr.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/glzfypnrr.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/getywvbsg.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/glcjakrrp.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gkjunegup.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gufdyzkmx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gziocwzqr.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gngjoqqhe.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gbzvxrphn.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gidigheii.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/gacxhuiiw.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gsvmzudkd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/gyvcxdotk.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gufuenejo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gnzfyufgm.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gkstzkpvk.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gfcyssjaw.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/glruwfprn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/gkoxgbzbk.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gjeuqtmaz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gpnlevkop.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gnkooigtn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gtneqhcmz.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/guoawysjp.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gfmdqqhds.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/ghyuauygy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gymjthpwn.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/guuxeuqvb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gfbdevylq.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gruwxqwlr.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gjysrmayu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gobdwvpzv.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gkkilxaje.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggjfuidcz.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/guufnbjhv.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/ggcwfpzql.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gqovdgokl.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gxwzodfmh.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gkkhrmrim.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/ggtyxwtdp.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/gfadnukyr.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gsmlqmcdx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gcezknqlw.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gwdxrorcg.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gtweguwww.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/gxvmdwrsc.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/gspzotbqb.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/ggcovopon.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gjhllfnym.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gyvafpdat.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gsswrcgki.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gobrzvpjq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gigkmehcs.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gtxqrxrit.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/givicnlyn.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gefsjffvg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gmhuhckoh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.zdbjq.cn/Article/details/gxjchxhjf.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/guguhijpe.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gvgwhljxk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gqqszuxjm.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gcxlceqff.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gzbojlfkx.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/ggghhbnyt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gllqlqhrh.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gbcbjsity.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gdhjizuvj.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gipmemosk.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gvfzfjmin.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gqtllfxpg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fehbvm.com/Article/details/gmhfpiuey.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/gploccyam.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gbnvpzazw.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gibknetro.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gjvrbwaks.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gwqffuluo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gxlgzriox.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/gtsbbsfep.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gntgexokm.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gzhgpflgs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gnkiplvth.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gqwxtvcho.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gcrgvipkd.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gvmjugflq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gkxoibrtr.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gmlttgxth.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gavpluipq.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gtdkhyxpj.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gayftfqed.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gtsudqvqj.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gjwidmaee.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gitysdxdt.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/glwgqfoza.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/gprjvocyg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gmpgblprm.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gmkcecjuq.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/gwntgeucn.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/ggrvxqpmn.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/guwioeqqu.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gkmpstlee.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/guxdmhpyi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gfgtcwpvv.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/geebucqax.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/gobsgnolz.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gqoobhpek.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/ggqgieedu.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gvgagrjar.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/gadeosdkk.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gvjoocnga.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gnntblqih.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gdpkutbll.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/ggmvjjwml.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gwoudnifd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gqxubtepx.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/ghmmswgkz.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gxlpcyahv.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gfovqzhfv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gtrlzfwqi.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gtgafjpjf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/guzchxrxe.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gjrqzhvcb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/ghibuygoh.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gdumdzsrn.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/ggsetieke.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gesiiysft.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gzfuvaiui.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gsakwsuao.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/geahctcom.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gjantwwlk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/gepqfufmo.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gevtxaizq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gflbrzdrp.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/gptrwqvtt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gjkdmubfn.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gefnuiohb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gvptlqpfw.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/genrfxnqc.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gefamypvu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gzwaujkqu.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/goicpbzik.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gtnrqhpny.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gvonnzrdl.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gnaiqagep.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gcuijnvfc.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/gpkcorzod.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/giqtyvdfk.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gemqldspp.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gvudljgcl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gyqfxtvei.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gvxwriznw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gtzumahjj.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/geabxolsw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gbkvmxzdy.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gpypyvfna.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gvnowhzsr.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gxzeuudga.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gqarxmjkl.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gwpmafbvy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/ggmghcbvo.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/geketqavz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gbcxmgkhf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdvifrrwl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gpxilusmr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmkivflar.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gczhuacep.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gmuyrvggy.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gawflfclq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gxapmayxa.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/glnphvvli.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gzutxafts.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gbqvakuqj.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gwjpkboev.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gkadushul.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gngoqient.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gftundaan.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gntgruiol.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gzrbslzhv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gwnbydjhm.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gdhawnzip.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gyoqgxjqr.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gzbomssmf.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gkrhyivlv.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gizswmqgx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gklcwpeeg.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gmktwjfkl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/glrwdrhoa.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gwkmpkjjw.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/girshmyzh.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gqszdcrfw.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gpwopayjp.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gxacidfxg.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gojbnlmko.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gmmzfcxor.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gkkmcxcwg.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gowkwkmlt.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gfasxaahd.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/gecnnvszv.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/ggtnfrids.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gajtsdwgm.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/ggksjybpk.sHtML


<!-- 参考信息 -->