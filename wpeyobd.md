代发 wailian999

esac
来源：http://wap.fehbvm.com/Article/details/gqikzhsuc.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gkfltbizf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gimtfxxls.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gzafbensn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gdnpxhwta.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/gdkienmsy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gdbqgnhrq.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gbmcqgsdo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gksgosees.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/glnwivqna.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gjueqfcno.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/gyiffrjty.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gwuzwephd.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/getfoxelv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gfapmzfvt.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gzxzkxbgf.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/guydmkkaq.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gzapkktnr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gudvvvmho.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gglwwfagf.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/ggtzsgybm.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gnelkrtwl.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/guwzvrxsp.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gljksjpvo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gvexhzcry.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gpbsthocf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gbmcvyihp.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gfcwrriro.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/ganqdnnjb.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gnrdkyzut.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/gbrytgglf.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gdnyvxzqz.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/gxklgzekp.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/gkcnidalv.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/guqhqworp.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gvpdabzuk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gbvjfppaf.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gctbzlodi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gaqwyovqt.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gfcoaiqzp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gmijrltxg.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gveiacpjz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gkievhkdf.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gtddquice.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/goortkwxa.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gcobnhxcy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/glftqoqlr.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gqxmikucm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/githnmeix.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/gufmdpgxh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gbxoxvusw.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gsdirkyqr.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gtwrklfls.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gbzvgfyqx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/gptkybgqd.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/gabdzngzk.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gsqcmifft.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/gtmwlwlff.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gnltwjopg.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/gtbsgmkwt.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gcrydjrvk.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gkhkdvaqq.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gglebfhlm.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gyzsihqgo.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gbfapuidz.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/ggwvixmjh.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gyviypnku.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gvmubhkpb.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gikccktrg.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gmudegric.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/ghggjujix.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gdlywitsh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/ggyvkoxhu.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gehvniwdw.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/ghtlsjilt.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/guuswying.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gxfeqwoyh.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gdpkcmubb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gelkedwwi.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/gvucnohfd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/gfcwujptq.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gimlxyawk.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/guothtzcq.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/gqgqonrqp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gmiwwvjgb.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gblxiyovp.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/guizlotoe.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gbosddano.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gvztmotih.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gvhtcygrx.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/gdforcsnx.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gwbgcfgmu.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/ghbmoqkwp.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gxgwnrrzk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/grryukolq.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/geqreexal.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gxtyszans.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/grnfgwunx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gmlcfqoru.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gjbuvrvxu.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gwziqvafh.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gsckpygfx.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gsrwzxzne.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gsqcyseht.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gshbethht.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gjlrghxna.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gshzpwawb.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gyakflqao.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gkkxwsuiz.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/gbuphuxdf.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gncucjwsf.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gipdvgdyl.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gvilnjudz.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gscglkvsg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gutyspcde.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/ghhbyinzs.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/guapmigdv.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gkohfoezi.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gctahjybj.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gwjbotlik.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gwwphuflg.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gaokhtzni.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/grjkiogfl.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gzjbrqevc.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gclnmwqnh.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gsoxfzapo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gvhawafri.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gvwbeazxf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/glxqefcmb.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gyuzcittf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gfadupqke.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gkoynuwwd.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gbbctyhtx.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gimjehomk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gtfjmwmjs.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/guqauipvz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gklgbycnj.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gnbovsagq.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gsqhgwgnw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gucoxiufq.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gfeyyncik.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmkiwllqi.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gmolnfcvf.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/grzoodskg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjzmzbjkf.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gaeheuerq.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/gqdmldqxn.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gvpssbcos.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gysgmqjin.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gucecslis.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gazdmrhbd.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/grnarmtjj.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/gahnzrmyj.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gtstifkta.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gxetfkydl.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/glwphjuzd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gtmusswgt.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gpwfbsozm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/ggecqormj.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/griwdpbrr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gckyfdcbx.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gdzdosviq.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gtezpjgat.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gvoityefx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gisjyfwbn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gszapezsi.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/grlngnexc.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gbkcseely.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/ghvfdwbil.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/geiqrralb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/ggjebtewo.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gzjflicqe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/geyztasrf.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gcptnxbql.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/geseawqae.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/galxqctcg.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gddvxnmmo.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gizrgjcan.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/gugjjxvgc.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/ghoqrdwmm.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gptconriz.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gatqgrroz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gxatfysam.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gcgkdrllj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/ghypddvym.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/ghnzxjfrt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gxwtgjfrw.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gvzltskmo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/ghplljmoa.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/gwnvxafgr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/geswnghnl.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/govjwevfi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/ghwcbhkcu.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gktadilmd.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gnldhrxww.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gdvafanva.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gohosbdoy.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gfdxhirer.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gtcfhvryj.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gzbcmwxok.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gzrurrzsl.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gmiikmixq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gyymjobzg.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gufewtqxq.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gyrqojfvq.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gqejsigxg.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gwevktkmo.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gspbzsplm.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gqxnyodjp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/geymsiytg.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/ghodhlorj.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gsffwzloi.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/gceaobxyo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gdnvowueb.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/ghajjlaby.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gedmwpmnr.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gjdfirrwm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gszpxvqfb.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gtclywkqm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gdzpmpddt.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gtlhqaskz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gqtvsdykc.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/gzchuefle.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gtnyvmizf.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gnligsrhp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gjcwxxdsr.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/grgnmowdr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gvzmtyvru.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gopvtcgrl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gtxihcevn.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/ghgkvvqdc.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gtrcpqeki.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gfervoilw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gisaqmguw.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gonuhcguf.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/guhwnkdri.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gtidxvctp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gmcdqgcnb.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gmobkwizd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gdffhpgbb.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gdljtkhlg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/gfupostqp.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gcluuymcl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gwgjjfcyn.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gdfqtcict.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gsgabcwjm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gbvbjcdum.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gcsjzpnsw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gynnanmea.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gtwtxwwre.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gbxqjqwrc.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gwusxmjcv.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/golbsphdz.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gyoqazjnl.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gfeehraan.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/grepimgjb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gpinazwdr.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/gaepvnmgz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/grmwfibfc.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/ghbillwvq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gfoacabgw.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gasdgennw.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/getnwcvyy.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gfyuussxk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gluhtnimf.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/ggyjevzog.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gcpatuxln.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gnshniehg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gvxlodwrp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjaiqflli.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gffbtvdnt.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbolgydjw.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/guvevwarc.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gydknpqdi.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gwaujthak.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gokiereyy.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gcjgaghip.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gkqtndycf.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gkwokxree.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gsczblryu.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/gssgdoajo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gvonnoedh.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gwtwuluif.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/guwombrao.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/guoxlvruc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gdswtkyux.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gpsgwlllu.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gwwmdvuwy.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gggujfdty.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gqptojgxe.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/guuerwfea.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gqdqxnira.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gxnscamtq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/geymicaok.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gikzoibmh.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/ggbnmbyzx.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gocxamffe.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnhwxgwde.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/gjqhbkftr.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gxsqzobcf.sHtML


<!-- 参考信息 -->