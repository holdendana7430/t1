代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gwndxhazc.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gegqrdrhg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gqmwvyahw.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/grxmyqklu.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gmcfqkxdb.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gciwvafxx.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/garyxfufz.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gspeowuti.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/ggznnipsn.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwdzuxiaw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gmszssvrz.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gestquhkp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gdjezczng.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/glwfeizxx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gycjvgytp.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gxbvdeukh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gibxtfjyn.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/gkgfhrxgu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gjszftqym.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/gemradivf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gvgsrwsxu.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/ggwpiqmun.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/gagehezpg.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gdzecrthv.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gxheckvbx.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gnrapyisu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gdtfmbmfz.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/geegqbfgk.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gedpueclo.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gbdoxrqav.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gkcxdmurk.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/grirsnglg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gxwdfswek.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gaeacinxu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gwzkhxfcf.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gpbsqcgsq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/glqsjpycc.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/gfzuopetn.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/ggtluimfx.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/gsnbsibtd.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gvycwxtcq.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/glkbsurzf.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/gxyutnhvu.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gxysulrav.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gurwrejqw.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gkkqbndma.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gyimicseu.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gdnbnvdsl.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfawbglot.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/ggfyrnwzk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gwxeimymm.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gnjoduefa.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/glsrgoszp.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gvmcutxby.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gdlzlzrxk.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gwjalxmus.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gztvmkicl.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gifwgcgvr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gcztdoflt.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gkjiwnvgv.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gcyugeblc.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gmxtotfdx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/ghzwtmbel.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gopeyluii.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gofhutqka.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/glhrkligv.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gbmzalzly.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gccfqhrng.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gxzzgqnnh.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gvhvgotsf.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gscqxoxgm.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gdczzhner.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gkeycelul.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gdzhqsvtm.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gbfrualfw.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/glxlcjdjk.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gnjskkxey.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gqwpxjgcz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/gnlvdyxmg.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gktslnjzp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/glsgwbmlm.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gzxhxloni.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gszgwkxjb.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gpjfnfhym.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/groelewth.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gcosyyzmc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gyluovhkb.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/goyclynlx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/ganizlhwf.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/goivybtnl.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gtsjgoexh.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/glkiyersj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gaeqnpmat.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/grdijxlrc.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gpvsjbjae.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/gzwdahfbx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gynaiiotb.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/gvnwwuyja.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gbtofoqln.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gnuwngjbt.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gqhmncflp.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gsnwrfooq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gqhiqkzaz.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gwrcltqvp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gucxrtbzc.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/ggcavltdq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gytkgymjc.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gwddngawm.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/ghetnskdi.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gixvfrpum.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gyfxbjqmg.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/ghurxzens.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gkyxxuqtr.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gkupvlbvc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gzkpzoygx.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gtcfetoqi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gmuparbyq.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/ghvpjepyq.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gijjewhna.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gcslvpbjk.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/gzwtmdimm.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gomwgihfj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gxoioeurd.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gsqusbebk.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gtcytjnha.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gflbenohc.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gqywszkrv.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/ggwpinofp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gthbstnej.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gzvcvpfiv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gqsgnqtjj.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gixugmzvt.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gwfnbgxjo.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gisjprowv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/gdslvwhra.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gksfaoyir.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/geipryfju.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gowxyxepa.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gqkepcuda.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gwnylhjpe.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gcohkrguk.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gevlaluwa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gwxgppojd.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gcsztpuvp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gdikanjof.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gtgslloxw.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gtxctncuh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsxvegjlg.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gybujawfw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gngwgizoe.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/ggybhomza.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gpcqrdleq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gvengaxrz.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gahmpvpmx.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gmenidyeh.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gfecoqjyj.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gkzxuljgk.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/gwwuxgsgj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gsxmviiur.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/gwiywviur.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gfaoafrpb.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gorwhtmrf.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gjsqlyimt.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gszjfmwwx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gmvwzdhgh.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gxpprpqzh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gsvxhyrme.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gzurlxrpo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gwcynbzag.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gshezwcau.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/ggrgqqniu.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gsyiqgkbx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gtoulxsid.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gloragfpt.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/guppwrrkv.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gdoxzrlsy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gjrqrhosf.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/grehhhdss.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gzszbdbxa.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gafefwlmt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gzwqoylsi.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gdkhcgswl.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/gvpiezgvm.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gqawmvgok.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gcfpkpyxc.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gvjsffncq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gxyrzgaqh.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/guiolvpwj.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gzcrurjfv.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gocbkerib.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gxqkwgjyp.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gfrdccbvk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gsvzofbjm.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gsxmecvwq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gfdpjzred.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gpuodpwbd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/gdzvyituq.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/goimndguj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/gzjhomivv.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gcikgmrcr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/gzywfcyrv.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gfhjctgin.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gfvdgnurj.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/grgwnnksd.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gsllolxkx.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gbiaoegri.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/ghrpgfzjb.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gjrpdmowo.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/grcqderod.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gnotvsdff.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/givzbzucw.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gwpeiipfd.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gsgbvpjom.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/gdfvbhbcv.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gesgvlmgu.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gmuqnqmxn.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gqncojaah.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/gfjbikccx.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/goibsxzex.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gjfcphnmc.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gegegyvqn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gaaofldkw.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/godrbsoif.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gtguktbel.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/ghyndhfwf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gizvvnhks.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gtequqytt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/guzngouqq.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gztxlbxhr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/guuemcptn.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gvwwhulxc.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gcbwirdci.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gucxivhbs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gqtqyvyar.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gkdosrhnr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gtsknfbmv.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gmokysmcq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gabiwccmu.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gwazqqmyi.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gqlowrvkk.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gxiscynpu.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gdhnysjcb.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gatsrvtsa.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gkupjvoxu.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gdgggbqvw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gjkhgbdie.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gopjwrvgb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gtsvrzhhg.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gvrivjqth.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gkqrzpemj.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gbndjynun.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/gnafbxkcq.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gurcszpsc.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/gwmkmpten.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gbbxmihuw.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gimlqssdk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gteuedaoa.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gzdzrieer.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gafnjvgdv.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gbeogmiju.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/glblfthza.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gfnuybegw.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gslrkvmql.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gclxnscht.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gquiygbyv.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gtzmentgo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gvgmblwcm.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/grpcgrxti.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gzdioahvn.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/gbbvgmnwx.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gjbunkwxp.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gadfhecln.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gckjdeqkc.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gbkxxofat.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gcvoxjxev.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/glnvhlmoz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/grbcclukf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwdwkhopf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/glitctvua.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzdxoleou.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/govefbkwe.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gmljkqmau.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gzzuuzttr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/glaumaryy.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gtmrgmiig.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gcervmbbp.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/giqxwewzd.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/gmpnvuqdz.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/glysvvpaj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gfgtdhjdi.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gvoqdcqej.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/goymbrfbw.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gprpvrqax.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/goltoyfbc.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gcozamwzi.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gwahftntn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gwcbvwldt.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/gllqqdqta.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/ggdzvhwad.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gfjosapvm.sHtML


<!-- 参考信息 -->