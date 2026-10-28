代发 wailian999

name="${1:-default}"
来源：http://hz.yonumen.top/gtpjylhewf.html

[R06] 判断命令是否存在
来源：http://hz.jlsjyb.cn/gtcfynnavn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.bjfxy.top/gtocxcrqxj.html

[R07] if 判断文件
来源：http://hz.hongshengwenyu.top/gtujxeccwy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.cashguo.top/gtyuyewhiz.html

[R08] 数值比较
来源：http://hz.316326.xyz/gtazboenbi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jiagoushi.top/gtzcvnhkev.html

[R09] 字符串比较
来源：http://hz.fzhhl.top/gtntnyvfqj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.daxiang520.top/gtdhfchrjf.html

[R10] 正则匹配
来源：http://hz.yj202588.top/gtebzoatpp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yj20258.top/gtqedsbesq.html

[R11] case 多分支
来源：http://hz.birdmap.top/gtertqhoua.html

case "$1" in
来源：http://hz.xuetiantiany.cn/gtuqwkgmua.html

start) echo "启动" ;;
来源：http://hz.316326.xyz/gtpsvnubwk.html

stop)  echo "停止" ;;
来源：http://hz.pycfn.com/gtpudwvxnl.html

*)     echo "未知命令" ;;
来源：http://hz.sweek.top/gtbloamcbk.html

esac
来源：http://hz.c1oappe.top/gtvdozccnn.html

[R12] for 遍历文件
来源：http://hz.tianlin.xyz/gtbpjtwzji.html

for f in *.txt; do echo "$f"; done
来源：http://hz.shuidangran.top/gtkqgvwhfy.html

[R13] for 计数循环
来源：http://hz.feifeiyinyue.top/gtactwliwf.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.iojbl.cn/gtgdznidbt.html

[R14] C 风格 for
来源：http://hz.xinyue.icu/gtdbmaubab.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhixingplan.top/gtxccpaoog.html

[R15] while 逐行读文件
来源：http://hz.havefunace.top/gtxtomiuue.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xingfuxueyuan.xyz/gtdvinceyk.html

[R16] until 等待条件
来源：http://hz.feifeiyinyue.top/gtecmmisdz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.sufxvd.cn/gteaxfmhzq.html

[R17] 数组定义与取值
来源：http://hz.jinghuilouyu.cn/gtfwmjarfa.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.daria6918.cn/gtvpgbwtqc.html

[R18] 遍历数组
来源：http://hz.hammf.cn/gtaujcctot.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.birdmap.top/gtkmdxzrkm.html

[R19] 数组长度
来源：http://hz.wangshuangyany.cn/gtmptzqykx.html

echo "${#arr[@]}"
来源：http://hz.gogol.net.cn/gtgdrixjez.html

[R20] 关联数组（字典）
来源：http://hz.iojbl.cn/gtuwjmuirk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhoulong.xyz/gtworiammf.html

[R21] 字符串长度
来源：http://hz.zycfv.cn/gtndzooyzm.html

echo "${#s}"
来源：http://hz.zhijiandao.cn/gtkpqtmlsj.html

[R22] 截取子串
来源：http://hz.yongpay.top/gtgethdcwb.html

echo "${s:0:5}"
来源：http://hz.ppjwa.cn/gtvbkltfzt.html

[R23] 字符串替换
来源：http://hz.ydjk.org.cn/gtceecamwp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yueranfly.top/gtgljhixdt.html

[R24] 大小写转换
来源：http://hz.xziqi.cn/gtdvsbrdjc.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.vqdsnc.cn/gtrbwwpytl.html

[R25] 去后缀 / 去前缀
来源：http://hz.iojbl.cn/gtrihooegj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ehwqpu.com/gtczulrxyd.html

[R26] 命令替换
来源：http://hz.xuanzx.com/gtnwtekgcq.html

now=$(date +%F); echo "$now"
来源：http://hz.pengpengdd.cyou/gtrepneldh.html

[R27] 算术展开
来源：http://hz.guowangkeji.top/gtavfflrin.html

echo $((1 + 2 * 3))
来源：http://hz.meibo888.top/gtbvsdzlii.html

[R28] 浮点运算
来源：http://hz.yueranfly.top/gtlwugipar.html

echo "scale=2; 10/3" | bc
来源：http://hz.cucudq.cn/gthrkndaux.html

[R29] 定义函数
来源：http://hz.vqdsnc.cn/gtregunpud.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.fzhhl.top/gtbblszfxx.html

[R30] 函数返回状态码
来源：http://hz.zhixingplan.top/gtmtnvqguf.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jinyuanbaomall.cn/gtltkpsqeq.html

[R31] 局部变量
来源：http://hz.yonumen.top/gtnfxkdrby.html

f() { local x=1; echo "$x"; }
来源：http://hz.kuanghao11.cn/gtwajrcfhe.html

[R32] 参数个数校验
来源：http://hz.gaohongyu789.top/gtlliuuzdq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cashguo.top/gtzxvlorkx.html

[R33] 捕获错误并提示行号
来源：http://hz.tanke756.top/gtwsbkoxnv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shzxlz.cn/gtygyvgzka.html

[R34] 退出时清理
来源：http://hz.andypj.xyz/gtkoigthak.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.cqqwz.cn/gtubzckpdw.html

[R35] 后台执行并等待
来源：http://hz.sxryk.cn/gtzpossaju.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xylfe.cn/gtkwtdsscw.html

[R36] 并发执行多个任务
来源：http://hz.aizwys.cn/gtddtsvqua.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yueranfly.top/gtxwtzfhok.html

[R37] 把输出赋给变量
来源：http://hz.sxryk.cn/gtffdaxydp.html

files=$(ls -1)
来源：http://hz.zhengqikj.top/gtrgsdnhiy.html

[R38] 管道串联
来源：http://hz.tian-w.cn/gtgbldsikf.html

cat a.txt | grep -i error | wc -l
来源：http://hz.xylfe.cn/gtmvopxyml.html

[R39] 重定向标准输出与错误
来源：http://hz.yj20258.top/gtgkqskyrs.html

cmd > out.log 2>&1
来源：http://hz.chenzaomai.com/gtvuyxkzti.html

[R40] 追加写日志
来源：http://hz.smart0.xyz/gtxwfjyspm.html

echo "log" >> out.log
来源：http://hz.meibo888.top/gtfzjqqmhl.html

[R41] 丢弃输出
来源：http://hz.nanxinkj.top/gtelijjqlh.html

cmd >/dev/null 2>&1
来源：http://hz.zhongyouzk.top/gthpvjtriu.html

[R42] 输入重定向
来源：http://hz.guowangkeji.top/gtwzuxqsao.html

wc -l < a.txt
来源：http://hz.jinghuilouyu.cn/gtnmvvggko.html

[R43] 按名字查找文件
来源：http://hz.ywan-chungtsiang.top/gtyyewilpg.html

find . -name "*.log" -type f
来源：http://hz.jlsjyb.cn/gtwzstxdng.html

[R44] 按修改时间查找
来源：http://hz.yj20258.top/gtbhwxamzr.html

find . -mtime -7 -type f
来源：http://hz.cdnleiting.top/gtkehcyllo.html

[R45] 批量删除
来源：http://hz.daria6918.cn/gtknhvjwkt.html

find . -name "*.tmp" -delete
来源：http://hz.pengpengdd.cyou/gtmiiesojd.html

[R46] 递归替换文件内容
来源：http://hz.ydzc1.top/gtxwbpsljv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ivvv.top/gtsorjuyrx.html

[R47] sed 单行替换
来源：http://hz.vqdsnc.cn/gtbwhgvgzc.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.sufxvd.cn/gtqfpijqut.html

[R48] awk 取指定列
来源：http://hz.smart0.xyz/gtpdclvcqw.html

awk '{print $1, $3}' a.txt
来源：http://hz.dianchejie.cn/gtyxglgazy.html

[R49] awk 带条件
来源：http://hz.chenlongwang.top/gtsppstcpx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xylfe.cn/gthgwenhis.html

[R50] awk 求和
来源：http://hz.wangdashe.top/gtqxwnuyoi.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yj20258.top/gtfkdhrxyx.html

[R51] 排序去重取前几
来源：http://hz.daxiang520.top/gtqmrkfdoe.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhaomingkeji.xyz/gtpsphjzno.html

[R52] 统计行数
来源：http://hz.quarkkingdee.top/gtdgsmokru.html

wc -l a.txt
来源：http://hz.zhijiandao.cn/gtbmcwaevm.html

[R53] 查看文件头与实时尾
来源：http://hz.tian-w.cn/gtlbpzoewd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yj20258888.top/gtbscgabvz.html

[R54] 比较两个文件
来源：http://hz.yueranfly.top/gtwcsiyxge.html

diff a.txt b.txt
来源：http://hz.fengsongda.top/gtjrwmqejd.html

[R55] 压缩与解压
来源：http://hz.aizwys.cn/gtckgyqlhz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jinghuilouyu.cn/gtbkbtdqra.html

[R56] 远程拷贝
来源：http://hz.chenlongwang.top/gtwkjovlff.html

scp file user@host:/path/
来源：http://hz.9152youxi.cn/gtbjzwbcna.html

[R57] 远程执行命令
来源：http://hz.cucudq.cn/gtyhxaqdxw.html

ssh user@host 'uptime'
来源：http://hz.cucudq.cn/gtwetsixhc.html

[R58] 下载文件
来源：http://hz.hysaishi.cn/gtpanvoaoo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.mhx1999.top/gtxvxscyhk.html

[R59] 发 POST JSON
来源：http://hz.hywenlv.cn/gtsijddrli.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhengqikj.top/gtmtwncbvd.html

[R60] 只看 HTTP 状态码
来源：http://hz.sysykeji.top/gtvmgdyqac.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.pengpengdd.cyou/gtjsvpbfqi.html

[R61] 磁盘占用
来源：http://hz.vqdsnc.cn/gtogvpjtus.html

df -h;  du -sh *
来源：http://hz.xingfuxueyuan.xyz/gtcbynsbze.html

[R62] 找最占空间的文件
来源：http://hz.pengpengdd.cyou/gtixxgoltz.html

du -ah . | sort -rh | head -10
来源：http://hz.ywan-chungtsiang.top/gtqtbasdet.html

[R63] 内存与进程
来源：http://hz.yongpay.top/gtoqumiuki.html

free -h;  ps aux | grep nginx
来源：http://hz.daxiang520.top/gticbsbafd.html

[R64] 结束进程
来源：http://hz.meibo888.top/gthtckjtos.html

kill -9 $(pgrep -f app.py)
来源：http://hz.gotoacloud.top/gttrhksrgp.html

[R65] 查看端口占用
来源：http://hz.guowangkeji.top/gtxtmbsoop.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.meibo888.top/gtshcmbaqz.html

[R66] 定时任务
来源：http://hz.chenzaomai.com/gtyukwvsxu.html

crontab -e;  crontab -l
来源：http://hz.fengsongda.top/gtwetlcgnw.html

[R67] 生成随机十六进制串
来源：http://hz.yonumen.top/gtauuskfsg.html

openssl rand -hex 16
来源：http://hz.redwolf501.top/gtadrciioy.html

[R68] 计算文件校验值
来源：http://hz.shuidangran.top/gtrsbotggu.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xingfuxueyuan.xyz/gtloymxfxh.html

[R69] 生成随机密码
来源：http://hz.sweek.top/gtcgdvkpkw.html

head -c 16 /dev/urandom | base64
来源：http://hz.snrcjt.cn/gtyqgfnahs.html

[R70] 时间戳与互转
来源：http://hz.cqqwz.cn/gtrnyvasub.html

date +%s;  date -d @1700000000
来源：http://hz.yangfankeji.com/gtzcnjpdcj.html

[R71] 日期格式化
来源：http://hz.chenlongwang.top/gtvcqzfibr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.nanxuanxn.top/gtnggnezin.html

[R72] 等待端口就绪
来源：http://hz.yongpay.top/gtrmoezxmt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.wangshuangyany.cn/gtovdeywhs.html

[R73] 分割大日志
来源：http://hz.cqqwz.cn/gtapcqwxzo.html

split -l 1000 big.log part_
来源：http://hz.hfpthk.cn/gtnseznqql.html

[R74] 批量重命名
来源：http://hz.xuanzx.com/gtmrgwlpku.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.birdmap.top/gtspvfmacz.html

[R75] 导出环境变量
来源：http://hz.feifeiyinyue.top/gthqtvbmmp.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhijiandao.cn/gtsvimtqoo.html

[R76] 使用临时文件
来源：http://hz.fengsongda.top/gtpbgdmcpr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinqigufen.top/gteuesydgd.html

[R77] 读取用户输入
来源：http://hz.yj20258.top/gtaxsjarlz.html

read -rp "请输入: " ans
来源：http://hz.guowangkeji.top/gtufuawqnt.html

[R78] 交互式菜单
来源：http://hz.52xcode.cn/gtvfwjjhyl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhengqikj.top/gthxyxcyvz.html

[R79] 解析命令行选项
来源：http://hz.jqgufenzy.top/gtkwyhafjo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yangfankeji.com/gtqzyhkgyc.html

[R80] 查看脚本执行耗时
来源：http://hz.jianghu66.top/gtxzilybsq.html

time ./run.sh
来源：http://hz.ppjwa.cn/gtecwtxcxg.html

================================================================================
来源：http://hz.tianlin.xyz/gtcuppxqvh.html

S. C / C++ 专题
来源：http://hz.birdmap.top/gtolgcfgno.html

================================================================================
来源：http://hz.ppjwa.cn/gtqdivqqub.html

[S01] C：Hello World
来源：http://hz.tanke756.top/gtmkrtqhac.html

#include <stdio.h>
来源：http://hz.hongshengwenyu.top/gtlqxnklct.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhiwuduotai.top/gttkkvyazs.html

[S02] C：变量与格式化输出
来源：http://hz.jinqigfzy.top/gtgvnqeyph.html

int a = 10; printf("%d\n", a);
来源：http://hz.yongpay.top/gtzceeajvd.html

[S03] C：读入整数
来源：http://hz.zhoulong.xyz/gtdlobcnro.html

int x; scanf("%d", &x);
来源：http://hz.wangshuangyany.cn/gtbytdyamr.html

[S04] C：字符串复制
来源：http://hz.cashguo.top/gthzqhfhmu.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.shanyushiyangtech.top/gtrchzaznz.html

[S05] C：字符串长度
来源：http://hz.ehwqpu.com/gtncpdhfhr.html

strlen(s)
来源：http://hz.kuanghao11.cn/gtraqgzwpp.html

[S06] C：字符串比较
来源：http://hz.chenjidiqi.icu/gtnnwshwck.html

strcmp(a, b) == 0
来源：http://hz.wangdashe.top/gtvcgmafbn.html

[S07] C：数组遍历求和
来源：http://hz.dashuyun.cn/gtzasomtag.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.chenzaomai.com/gtcxjvwqml.html

[S08] C：动态内存分配与释放
来源：http://hz.jyoumei.cn/gtcrujbldp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.cheryme.top/gtgfkwjfjt.html

[S09] C：结构体定义与初始化
来源：http://hz.sufxvd.cn/gtecrrbqss.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xylfe.cn/gtrzksijaj.html

[S10] C：指针与解引用
来源：http://hz.sweek.top/gtqfckgmfy.html

int *p = &a;  *p = 5;
来源：http://hz.hysaishi.cn/gtyfkljqxi.html

[S11] C：逐行读文件
来源：http://hz.cheryme.top/gtuqzpwnut.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jlsjyb.cn/gtqzmsobzb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.cheryme.top/gtecshhajk.html

fclose(f);
来源：http://hz.ehwqpu.com/gtyoisdhol.html

[S12] C：写文件
来源：http://hz.jinyuanbaomall.cn/gttnkyiqeg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.dashuyun.cn/gtyzuourgr.html

[S13] C：宏定义
来源：http://hz.pengpengdd.cyou/gtvecmexei.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yj20258.top/gtiqggyony.html

[S14] C：枚举
来源：http://hz.redwolf501.top/gtmnfpykmc.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhaomingkeji.xyz/gtxvvokpqb.html

[S15] C：类型转换
来源：http://hz.shuidangran.top/gtjvxbfpye.html

(double) a / b
来源：http://hz.xingfuxueyuan.xyz/gtjvvkqoau.html

[S16] C：位操作置位
来源：http://hz.zhixingplan.top/gtwpoenqkr.html

x |= (1 << 3);
来源：http://hz.mhx1999.top/gtfbvoelhj.html

[S17] C：安全拼接字符串
来源：http://hz.jinyuanbaomall.cn/gtjhhaxbvv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.cqqwz.cn/gtssewnqpr.html

[S18] C：命令行参数
来源：http://hz.hongshengwenyu.top/gtjtauksyj.html

int main(int argc, char **argv)
来源：http://hz.fengsongda.top/gtafaacylj.html

[S19] C：快速排序
来源：http://hz.guannengcc.top/gteffvxstd.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.ydzc1.top/gtjbxksisv.html

[S20] C：二分查找
来源：http://hz.feifeiyinyue.top/gtavketqda.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jianghu66.top/gtprneeyke.html

[S21] C：字符类别判断
来源：http://hz.svipenyu.cn/gtolkvhdxz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.cashguo.top/gtedncuscm.html

[S22] C：字符串转数字
来源：http://hz.zhiwuduotai.top/gtvdxwwtpc.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.pycfn.com/gtapqjnwzn.html

[S23] C：随机数
来源：http://hz.havefunace.top/gtjdcbxbqk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cucudq.cn/gtsaelvcbw.html

[S24] C：获取本地时间
来源：http://hz.ywan-chungtsiang.top/gtqvxqrtkj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.cqqwz.cn/gtueiihxwx.html

[S25] C：内存拷贝
来源：http://hz.havefunace.top/gtbjrgnuul.html

memcpy(dst, src, n);
来源：http://hz.jlsjyb.cn/gtiqiaaiwl.html

[S26] C：内存清零
来源：http://hz.dashuyun.cn/gtzogqaoyb.html

memset(a, 0, sizeof a);
来源：http://hz.yangfankeji.com/gthoeuyajg.html

[S27] C：定义常量
来源：http://hz.xylfe.cn/gtzaalvawz.html

const double PI = 3.14159;
来源：http://hz.zhiwuduotai.top/gtehwksbjf.html

[S28] C：静态变量
来源：http://hz.jinghuilouyu.cn/gtcoqolpfs.html

static int counter = 0;
来源：http://hz.fengsongda.top/gtfxsscbxb.html

[S29] C：变参函数
来源：http://hz.daria6918.cn/gtkkvhkqhe.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yongpay.top/gtsfelvbab.html

[S30] C：头文件保护
来源：http://hz.aizwys.cn/gtsqbzehqd.html

#ifndef X_H
来源：http://hz.vqdsnc.cn/gtbvxlseuo.html

#define X_H
来源：http://hz.kuanghao11.cn/gtradailbj.html

#endif
来源：http://hz.daxiang520.top/gtuairvcbi.html

[S31] C++：Hello World
来源：http://hz.tianlin.xyz/gtlozeqcvt.html

#include <iostream>
来源：http://hz.zycfv.cn/gtsuepewfp.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.chenzaomai.com/gtbeakhyxp.html

[S32] C++：字符串
来源：http://hz.shanyushiyangtech.top/gtmsvlccrx.html

std::string s = "hi";  s += "!";
来源：http://hz.bjfxy.top/gtjsecocpg.html

[S33] C++：vector 增删
来源：http://hz.jiagoushi.top/gtvzoastin.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.gzhubu.top/gtlhllnkpu.html

[S34] C++：遍历 vector
来源：http://hz.52xcode.cn/gtagivfyib.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cdnleiting.top/gtpofktefd.html

[S35] C++：map
来源：http://hz.yuxming.cn/gtnvdhixmo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jianghu66.top/gtyllfkpqa.html

[S36] C++：unordered_map
来源：http://hz.birdmap.top/gtvjkcxevk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shzxlz.cn/gtisgokhug.html

[S37] C++：set
来源：http://hz.xziqi.cn/gthttdwapo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.316326.xyz/gtqgtzyzhw.html

[S38] C++：排序
来源：http://hz.iojbl.cn/gtvokcpjft.html

std::sort(v.begin(), v.end());
来源：http://hz.kuanghao11.cn/gtkaawmhvp.html

[S39] C++：自定义比较器排序
来源：http://hz.redwolf501.top/gtvppqjoba.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shanyushiyangtech.top/gtmlngmpyn.html

[S40] C++：查找元素
来源：http://hz.jinghuilouyu.cn/gtazfhtkwv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.sysykeji.top/gtijywxqjy.html

[S41] C++：类与构造函数
来源：http://hz.aibaodan.cn/gtxrixzuwa.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.bjfxy.top/gtmoijbvrn.html

[S42] C++：继承与虚函数
来源：http://hz.yangfankeji.com/gtilpphkhq.html

class B : public Base { public: void f() override {} };
来源：http://hz.shuidangran.top/gtjbneymil.html

[S43] C++：智能指针
来源：http://hz.zhaomingkeji.xyz/gtodojzbth.html

auto p = std::make_unique<int>(5);
来源：http://hz.yvedp.cn/gteewcjtpy.html

[S44] C++：引用传参
来源：http://hz.dashuyun.cn/gtzxbvlpri.html

void inc(int &x) { ++x; }
来源：http://hz.feifeiyinyue.top/gtnubntoas.html

[S45] C++：lambda
来源：http://hz.zhijiandao.cn/gtzmmmepas.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.daxiang520.top/gtxoedeqvr.html

[S46] C++：函数模板
来源：http://hz.snrcjt.cn/gtxpaaoeca.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.aizwys.cn/gtmjdxbiae.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhixingplan.top/gttphypyls.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yuxming.cn/gtadydgoog.html

[S48] C++：逐行读文件
来源：http://hz.jinqigfzy.top/gtnamaytvw.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.smart0.xyz/gthlesaofp.html

while (std::getline(in, line)) { }
来源：http://hz.chenzaomai.com/gtrzoziyed.html

[S49] C++：写文件
来源：http://hz.aibaodan.cn/gthribcryu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.sweek.top/gtkktrbwce.html

[S50] C++：格式化数字
来源：http://hz.jqgfzy.top/gtirveskhv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.svipenyu.cn/gtaokhwrea.html

[S51] C++：显式类型转换
来源：http://hz.redwolf501.top/gtdyqxuxen.html

static_cast<double>(a) / b
来源：http://hz.cqqwz.cn/gtjolgdcbl.html

[S52] C++：const 与 noexcept
来源：http://hz.xziqi.cn/gtsdyheggx.html

int size() const noexcept { return n_; }
来源：http://hz.chenzaomai.com/gtupuafiyl.html

[S53] C++：移动语义
来源：http://hz.zhongyouzk.top/gtehuhygat.html

std::vector<int> w = std::move(v);
来源：http://hz.shanyushiyangkeji.top/gtofylavxv.html

[S54] C++：异常处理
来源：http://hz.shangyingyoupin.top/gthggmxjey.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.redwolf501.top/gtbgvdheoq.html

[S55] C++：结构化绑定
来源：http://hz.ehwqpu.com/gtyqtfhdgr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xylfe.cn/gtymeuochj.html

[S56] C++：optional
来源：http://hz.ywan-chungtsiang.top/gtrqlyjjmx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.fzhhl.top/gtvsjxilnv.html

[S57] C++：编译期常量
来源：http://hz.bjfxy.top/gtcuidihvp.html

constexpr int N = 10;
来源：http://hz.gzhubu.top/gtwdcbvubb.html

[S58] C++：命名空间
来源：http://hz.ehwqpu.com/gtyazwzycr.html

namespace ns { int f() { return 1; } }
来源：http://hz.xuetiantiany.cn/gtupbyepwz.html

[S59] C++：静态断言
来源：http://hz.birdmap.top/gtrknxchla.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.0kj1m.cn/gtyxipftqp.html

[S60] C++：遍历并删除元素
来源：http://hz.iojbl.cn/gtlvfiwcdo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.aizwys.cn/gtmgjxqphs.html

================================================================================
来源：http://hz.cashguo.top/gtgcbudpyv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xylfe.cn/gttuisbbyh.html

================================================================================
来源：http://hz.birdmap.top/gtfccdbkwp.html

[T01] Kotlin：Hello World
来源：http://hz.chenjidiqi.icu/gtfarstlce.html

println("Hello")
来源：http://hz.zhiwuduotai.top/gttbpxnjxq.html

[T02] Kotlin：变量
来源：http://hz.zhijiandao.cn/gtoknmoegy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.smart0.xyz/gtiusmoqia.html

[T03] Kotlin：字符串模板
来源：http://hz.jyoumei.cn/gtjrgutumj.html

"值: $b"
来源：http://hz.gotoacloud.top/gtubjtfgnu.html

[T04] Kotlin：空安全
来源：http://hz.havefunace.top/gtfvdntnoe.html

val n: String? = null;  n?.length
来源：http://hz.52xcode.cn/gtzuqjnngs.html

[T05] Kotlin：when 表达式
来源：http://hz.jinghuilouyu.cn/gtqtkabcry.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.wangdashe.top/gtjkernnwg.html

[T06] Kotlin：集合映射
来源：http://hz.vqdsnc.cn/gtbxuhkfaq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.xuetiantiany.cn/gttghjyqbg.html


<!-- 参考信息 -->