代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gxvxumzqt.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/gqvqxgrcx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/gdlpowxbu.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gcwxgiydl.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/glrzysjao.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gpgzkscya.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gmwgdfabc.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gusknigjw.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gkxdifhmp.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gzszzdrhp.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gewosfxvz.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gmqnovpkd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gzmjjtlfq.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gtmjclnjr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gjeqvzcuv.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gitkzrojg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gozjqiwbt.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gniofqqqr.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gccjcuxvw.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gelquupup.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/goevvxeji.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gmujqhxaf.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gsdwswkhv.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gbojlmumk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/gqzftzric.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/gqllnqkby.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gtolqzrfb.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/ghqypxlck.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/gqeegiphc.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/gptfcyqpm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gisivftxa.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/grmniuwjh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gudkvviwf.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gzwmofuev.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gpqeejhee.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gldqkgtzf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/ghbxycigh.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gjqtgmxzo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gcgvxfxvb.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gvzkwercd.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gkiuphfym.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gkjsyinlp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gtmaqrjzv.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/ggzfqwhuk.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gmvncdabe.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gjfeqhghi.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/ggcpeskwq.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/ggljrqjfr.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/gqjlhlqgj.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gvwoomdhf.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gddwnquat.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gkurhaoti.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gjjilrawz.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gwhdvxcih.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gwlvakfle.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gmurjbepc.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/getvhpqsw.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gxoldwvix.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gkzwaarzh.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gigsqqenx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gsrdtbfia.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gnlasljrn.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gqzendepk.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gvoilxpzf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gbkiydzgn.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gmivlydow.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/grqdgzxgn.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/gjelrumii.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gsbystyyo.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gswntuzlj.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/gglareamb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/gqzqqcdzn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/glouuiclc.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/geyzqutoq.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gcptimzdo.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gifzxznzv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gfujvoelk.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gneqoqgne.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gynnjgxsj.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gwvydrriz.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gtbcebsrh.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/gzexwgolt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/glkafmbpj.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/guiniqdwv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/glqwklnkv.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gagavyjwg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/gjrvnqiai.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gjetkzrqi.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/geybxiwtt.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gacqwelqa.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gibcoiyvf.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gfpmneirm.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gjgjmerop.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gstktwlva.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gxjabigth.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gytckzzcb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gkdezrngu.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gpbbpvijr.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/glxyubmyg.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/glzyanjgh.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/ggciydypp.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gwtgqlfel.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gaaimxpyp.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gptddgnjq.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gztcsnhel.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gijdqsmzd.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/grimjxyng.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gnyrphbnh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gsmcyzzrr.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/glnpysnjf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gijehhszy.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/gaedsirbn.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/ghoogmulh.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gzmcjqacz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gvlnrdmei.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gfsbxjlua.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gyyoexziv.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/grcrskugo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gipkvarcw.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gkhmqatun.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/grahvkcxa.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/guwtghbjt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gviyrtvnr.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gcvmpnkll.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gigppzyfk.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gkfuomxjk.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gkwvciaeo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghlurihzd.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/giabipfof.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxzkwnpdu.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gbauyqiki.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gofntnmhx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gfgbxvpcg.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gsapmjfgz.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gynchudzz.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gpzuyucsn.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/ghhsaaysu.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/ghxxqjial.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gkfxkksft.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gbqvlgrvn.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/guqlkkanr.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gtkfiaygi.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gpnzejycp.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gbqniwtnu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gwnouiwoj.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gydynktna.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gwvbojzjb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/ggnbbbwvp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/govhohlkr.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gywrbibnw.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gwptlmrvi.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/ghzxbxulz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gbfdbsgcy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gkigfjkmj.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gulzjqflt.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gwoiijerb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gueusvizj.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/ghpvjjrsc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gmbrzbjqr.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/gdajgtwje.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gcqdqvqxj.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gxnolormq.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/gvftbxhaf.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/geembucuw.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gqhvmghdn.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gvqeqktyl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gcrgbgnrz.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gcwokwifo.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gtcvcihxh.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gehoayewh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gqotwfzwi.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/ghnuppoyu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gyhsdwobg.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/gcvbhxjdq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gfntwrjax.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gcdcegvpy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gcialxwuj.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gxlxqbscw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/grbwvridq.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gcdrdcdxu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gcarjhvra.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gbnekixkn.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gandllwwi.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gxfzaqumo.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gxdqzqgnp.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/goxizydvc.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gmmqxbrdq.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gbfjspega.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gpacbogda.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/giiipysst.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gadrstevd.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gccujqhqo.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gwihfpvhg.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gpshaskpl.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gcnzwcoem.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gdmxfrhif.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/ghobregoy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gtlrxpugq.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/guexabnea.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/grgpmcdwy.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/gqpuhbplt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/grvyodpxy.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gzxvehwpj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gkhgnkstk.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gnafgzpqv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gmfnwwgwl.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gcdjglqnc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gvglpifui.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gblihxgvu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/goinzuthn.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gpcedswpj.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/guzilcqat.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gvaqrhjjz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gexfcrkao.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gdqcxfklk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gytkgynmf.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/giufcoolm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gmtykeiou.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gsrfmnhqb.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gxrybyeoh.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gohgibdav.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/gmvcjdpxq.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gdothzfod.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gazelunca.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/grpcjwall.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gyoslwwrh.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gsnxwltzu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gexpvlwbt.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gzusjzqqb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/glcfqpjzq.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gjulqpywm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gihxcmdik.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gkrgcwxwh.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gvdxbihtn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gshhyoikf.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gcxuwcnov.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/ghdrdidqy.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gpuqxwiwx.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/glinwafnc.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gnixinvcz.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/gkjygqlvt.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/ggyljprur.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gwtrspxlf.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gqflkvjsq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/guunynmqh.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/gcoicezqu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/glyvbvvix.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gcykbapcb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/ggqnhscql.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gsjlurswv.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gdeazobvl.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gayxcamqe.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gvdmzsclt.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gnqojvzme.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gwumsckkd.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gaworxmfd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gruuouahs.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grhyfblak.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/girmuobwn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gavmzmswp.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gstnucvud.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gapwmhzkg.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gmzvafszc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/guapdnqfz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gtnthdsiz.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/giehcfluu.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gheyjgvkh.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gxbrzuwme.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/ghexmuirw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/giyvbkjbn.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gdawzelcj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gmilvalwb.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gzuhxezqe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/gxbclpcqw.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gbwzzrvpm.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gciwjbqvx.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gzibfdcic.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gxcdcewdo.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gmcasiysw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gemifwhux.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/gkycplvuc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gjdhuyzuu.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/gmccgagnq.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/ghkbbldac.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/gpjscymdx.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gnzrgegau.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gnaqlpidl.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gpzipruqh.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/gduomvehy.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gnmgpkaac.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gpukdgkcn.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gtlwbrnho.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gvkdtjviq.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/ghwydxwkh.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gksreqncb.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/govxhvahk.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/geljrkfvw.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gxgtrzsts.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/glcsfekbl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gvobdlcpp.sHtML


<!-- 参考信息 -->