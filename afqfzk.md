代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.nwbrower.top/gtstsajvkb.html

[R08] 数值比较
来源：http://hz.yuanzhike.top/gtcwdmmztb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.aibaodan.cn/gteapqtbnk.html

[R09] 字符串比较
来源：http://hz.ydzc1.top/gtgroqpzyx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jyoumei.cn/gtotqhwxds.html

[R10] 正则匹配
来源：http://hz.pengpengdd.cyou/gtveyoblhn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.tian-w.cn/gtptxfocjv.html

[R11] case 多分支
来源：http://hz.shanyushiyangkeji.top/gtwochnxlc.html

case "$1" in
来源：http://hz.vqdsnc.cn/gtkziqherw.html

start) echo "启动" ;;
来源：http://hz.cheryme.top/gtckhztdnc.html

stop)  echo "停止" ;;
来源：http://hz.shanyushiyangtech.top/gtzqolhdkn.html

*)     echo "未知命令" ;;
来源：http://hz.iojbl.cn/gtiyybqsoa.html

esac
来源：http://hz.cashguo.top/gthedtjfkx.html

[R12] for 遍历文件
来源：http://hz.jinqigufen.top/gthzudeqct.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hywenlv.cn/gtepwlomgf.html

[R13] for 计数循环
来源：http://hz.snrcjt.cn/gtsyxdutxu.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.nwbrower.top/gtvhgvhwff.html

[R14] C 风格 for
来源：http://hz.cqqwz.cn/gtfvjjlqex.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhoulong.xyz/gtpnhhtets.html

[R15] while 逐行读文件
来源：http://hz.tanke756.top/gtxatczfkx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hysaishi.cn/gtmnqiblev.html

[R16] until 等待条件
来源：http://hz.birdmap.top/gtgufoqeqv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.nwbrower.top/gtilufrjvz.html

[R17] 数组定义与取值
来源：http://hz.zhengqikj.top/gtvuvbllwg.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hysaishi.cn/gtpdvyeddc.html

[R18] 遍历数组
来源：http://hz.yonumen.top/gtxiobmhpc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shuidangran.top/gtsidicdft.html

[R19] 数组长度
来源：http://hz.gogol.net.cn/gtdgxxkfkl.html

echo "${#arr[@]}"
来源：http://hz.yuxming.cn/gtvjymjfom.html

[R20] 关联数组（字典）
来源：http://hz.sysykeji.top/gteycinbjf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhengqikj.top/gtxyzqfzar.html

[R21] 字符串长度
来源：http://hz.gotoacloud.top/gtxhfpchsk.html

echo "${#s}"
来源：http://hz.gotoacloud.top/gtdizapkuy.html

[R22] 截取子串
来源：http://hz.daria6918.cn/gtvtbolxcf.html

echo "${s:0:5}"
来源：http://hz.jyoumei.cn/gtkppzwrnu.html

[R23] 字符串替换
来源：http://hz.zycfv.cn/gtgcvtmcpq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shanyushiyangkeji.top/gtjmgfudem.html

[R24] 大小写转换
来源：http://hz.guannengcc.top/gttadxbiei.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.redwolf501.top/gtsiozpqdy.html

[R25] 去后缀 / 去前缀
来源：http://hz.shanyushiyangkeji.top/gtzmzvcwkn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.gaohongyu789.top/gtpqvbngjy.html

[R26] 命令替换
来源：http://hz.tian-w.cn/gtaldpbyxy.html

now=$(date +%F); echo "$now"
来源：http://hz.meibo888.top/gtnqkzcutz.html

[R27] 算术展开
来源：http://hz.sysykeji.top/gttvmcncsd.html

echo $((1 + 2 * 3))
来源：http://hz.fzhhl.top/gtavtcbpgv.html

[R28] 浮点运算
来源：http://hz.gzhubu.top/gtpaxqcsxt.html

echo "scale=2; 10/3" | bc
来源：http://hz.feifeiyinyue.top/gtfsbhxcaz.html

[R29] 定义函数
来源：http://hz.zhixingplan.top/gtosjuyjuz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhijiandao.cn/gtcpmrrqcs.html

[R30] 函数返回状态码
来源：http://hz.hammf.cn/gtmgvgtgnm.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jinghuilouyu.cn/gtkberontq.html

[R31] 局部变量
来源：http://hz.gogol.net.cn/gtfhxuzcvn.html

f() { local x=1; echo "$x"; }
来源：http://hz.jinqigfzy.top/gtahtiecvw.html

[R32] 参数个数校验
来源：http://hz.yvedp.cn/gthhquziaq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhoulong.xyz/gtgkrxvphi.html

[R33] 捕获错误并提示行号
来源：http://hz.sweek.top/gtxiueehtt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.sufxvd.cn/gtfnyiqwam.html

[R34] 退出时清理
来源：http://hz.nanxinkj.top/gtvbqgmley.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.guowangkeji.top/gtwwvttwgk.html

[R35] 后台执行并等待
来源：http://hz.andypj.xyz/gtdgymkpso.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.fengsongda.top/gtkcalpsnx.html

[R36] 并发执行多个任务
来源：http://hz.aizwys.cn/gtdjvfxebz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ydjk.org.cn/gtqbzgjzlo.html

[R37] 把输出赋给变量
来源：http://hz.iojbl.cn/gtnvkckgbt.html

files=$(ls -1)
来源：http://hz.cashguo.top/gtxcpcoiqu.html

[R38] 管道串联
来源：http://hz.meibo888.top/gteckijyvy.html

cat a.txt | grep -i error | wc -l
来源：http://hz.snrcjt.cn/gtdquvyvtv.html

[R39] 重定向标准输出与错误
来源：http://hz.zhengqikj.top/gtwarkosxr.html

cmd > out.log 2>&1
来源：http://hz.shangyingyoupin.top/gtshfdglco.html

[R40] 追加写日志
来源：http://hz.daxiang520.top/gtseucepoe.html

echo "log" >> out.log
来源：http://hz.ivvv.top/gtfhoakrpg.html

[R41] 丢弃输出
来源：http://hz.sufxvd.cn/gtrpnidhue.html

cmd >/dev/null 2>&1
来源：http://hz.chenjidiqi.icu/gtrqkplbxx.html

[R42] 输入重定向
来源：http://hz.tanke756.top/gtimbdixqw.html

wc -l < a.txt
来源：http://hz.aizwys.cn/gteqevlchp.html

[R43] 按名字查找文件
来源：http://hz.shangyingyoupin.top/gttgecqsvp.html

find . -name "*.log" -type f
来源：http://hz.zhoulong.xyz/gtqbsgkftt.html

[R44] 按修改时间查找
来源：http://hz.fzhhl.top/gtpewfnknn.html

find . -mtime -7 -type f
来源：http://hz.gaohongyu789.top/gtiixsgzni.html

[R45] 批量删除
来源：http://hz.jianghu66.top/gtlyiuhbeh.html

find . -name "*.tmp" -delete
来源：http://hz.daxiang520.top/gtiankvwtd.html

[R46] 递归替换文件内容
来源：http://hz.ehwqpu.com/gtnptahtnz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.guowangkeji.top/gtyjbhezmw.html

[R47] sed 单行替换
来源：http://hz.ydjk.org.cn/gtwomfjmdd.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.0kj1m.cn/gtlmxdcttt.html

[R48] awk 取指定列
来源：http://hz.yonumen.top/gtrtnvpiec.html

awk '{print $1, $3}' a.txt
来源：http://hz.shzxlz.cn/gtzojnvrdi.html

[R49] awk 带条件
来源：http://hz.andypj.xyz/gtsztwmxyu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.cqqwz.cn/gtgbgedwji.html

[R50] awk 求和
来源：http://hz.redwolf501.top/gtsxjspbpv.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jyoumei.cn/gtyqsledwk.html

[R51] 排序去重取前几
来源：http://hz.jianghu66.top/gttwohhmfp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ppjwa.cn/gtclukxkfq.html

[R52] 统计行数
来源：http://hz.yuxming.cn/gtxfzcsebf.html

wc -l a.txt
来源：http://hz.jqgufenzy.top/gtiwtcidvz.html

[R53] 查看文件头与实时尾
来源：http://hz.guowangkeji.top/gtpqvdrcmm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yuxming.cn/gtbrioblgs.html

[R54] 比较两个文件
来源：http://hz.zhaomingkeji.xyz/gthtbwmfrx.html

diff a.txt b.txt
来源：http://hz.ehwqpu.com/gtbpibzxur.html

[R55] 压缩与解压
来源：http://hz.dianchejie.cn/gttnpceajj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.gogol.net.cn/gtnshtmfmb.html

[R56] 远程拷贝
来源：http://hz.jlsjyb.cn/gtkzeczskn.html

scp file user@host:/path/
来源：http://hz.zhijiandao.cn/gtclewmgzy.html

[R57] 远程执行命令
来源：http://hz.jyoumei.cn/gtpthhdfqk.html

ssh user@host 'uptime'
来源：http://hz.zhongyouzk.top/gtksgqhkzx.html

[R58] 下载文件
来源：http://hz.zdqjudy.top/gtyvthlrnh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.tanke756.top/gtegiuzpsg.html

[R59] 发 POST JSON
来源：http://hz.ehwqpu.com/gtngsawygi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.smart0.xyz/gtjflviqby.html

[R60] 只看 HTTP 状态码
来源：http://hz.wangdashe.top/gtbgyflbkm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhaomingkeji.xyz/gtkzrzwrcl.html

[R61] 磁盘占用
来源：http://hz.hnxiangtu.top/gtscvlytmy.html

df -h;  du -sh *
来源：http://hz.shzxlz.cn/gtnlrfafwa.html

[R62] 找最占空间的文件
来源：http://hz.jiagoushi.top/gtnzrnvskg.html

du -ah . | sort -rh | head -10
来源：http://hz.ydzc1.top/gtdeotvquu.html

[R63] 内存与进程
来源：http://hz.yanxiufei.cn/gtbdetylqu.html

free -h;  ps aux | grep nginx
来源：http://hz.zhengqikj.top/gtpmylbsjx.html

[R64] 结束进程
来源：http://hz.tanke756.top/gtkykxeuxb.html

kill -9 $(pgrep -f app.py)
来源：http://hz.meibo888.top/gtgwozhrlf.html

[R65] 查看端口占用
来源：http://hz.hnqzz.top/gtuyjeimul.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhoulong.xyz/gtdjjktkrw.html

[R66] 定时任务
来源：http://hz.yonumen.top/gtjbhqexes.html

crontab -e;  crontab -l
来源：http://hz.jinyuanbaomall.cn/gtzzhdonnl.html

[R67] 生成随机十六进制串
来源：http://hz.chenlongwang.top/gtpmwlpbrr.html

openssl rand -hex 16
来源：http://hz.chenzaomai.com/gtngltisyu.html

[R68] 计算文件校验值
来源：http://hz.yj202588.top/gtbyzfazat.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.feifeiyinyue.top/gtheczbdan.html

[R69] 生成随机密码
来源：http://hz.zhijiandao.cn/gtylmuaunu.html

head -c 16 /dev/urandom | base64
来源：http://hz.jyoumei.cn/gtpgplmssq.html

[R70] 时间戳与互转
来源：http://hz.bjfxy.top/gtfkltuuzf.html

date +%s;  date -d @1700000000
来源：http://hz.jqgufenzy.top/gtoprfvglh.html

[R71] 日期格式化
来源：http://hz.yvedp.cn/gtdwfihlca.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shzxlz.cn/gtverltpuk.html

[R72] 等待端口就绪
来源：http://hz.sweek.top/gtqdtxvizj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yj20258.top/gtbapxuytd.html

[R73] 分割大日志
来源：http://hz.xingfuxueyuan.xyz/gtsshrowdv.html

split -l 1000 big.log part_
来源：http://hz.sysykeji.top/gtwgsrtrxv.html

[R74] 批量重命名
来源：http://hz.yangfankeji.com/gtrdezdtej.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.meibo888.top/gtdxotkzee.html

[R75] 导出环境变量
来源：http://hz.jiagoushi.top/gtjomxundm.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.c1oappe.top/gtsqyxujni.html

[R76] 使用临时文件
来源：http://hz.cheryme.top/gtvrtkvszs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.tian-w.cn/gtybbtzerr.html

[R77] 读取用户输入
来源：http://hz.ivvv.top/gtigclfxvg.html

read -rp "请输入: " ans
来源：http://hz.shanyushiyangtech.top/gtaaxooblq.html

[R78] 交互式菜单
来源：http://hz.ydzc1.top/gtrpvmkklz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.guannengcc.top/gtrggijdgf.html

[R79] 解析命令行选项
来源：http://hz.fzhhl.top/gtubegiegq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.dashuyun.cn/gtujzujnzc.html

[R80] 查看脚本执行耗时
来源：http://hz.shanyushiyangkeji.top/gtlfcfiudo.html

time ./run.sh
来源：http://hz.tian-w.cn/gtbhrgbmmu.html

================================================================================
来源：http://hz.aizwys.cn/gtryqzyprh.html

S. C / C++ 专题
来源：http://hz.zhengqikj.top/gtawcgtwgt.html

================================================================================
来源：http://hz.cucudq.cn/gtlmbfkizi.html

[S01] C：Hello World
来源：http://hz.gogol.net.cn/gtbmovozdy.html

#include <stdio.h>
来源：http://hz.zhijiandao.cn/gtjlbxmqjn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.kuanghao11.cn/gtmejjxzml.html

[S02] C：变量与格式化输出
来源：http://hz.gotoacloud.top/gtvmjaypgq.html

int a = 10; printf("%d\n", a);
来源：http://hz.52xcode.cn/gtkgiedlaq.html

[S03] C：读入整数
来源：http://hz.yuanzhike.top/gtiaklleok.html

int x; scanf("%d", &x);
来源：http://hz.cqqwz.cn/gtppkkcuob.html

[S04] C：字符串复制
来源：http://hz.hysaishi.cn/gtjsprozch.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhaomingkeji.xyz/gtjuwrzitx.html

[S05] C：字符串长度
来源：http://hz.9152youxi.cn/gttgomhdaj.html

strlen(s)
来源：http://hz.gzhubu.top/gtzpzbutex.html

[S06] C：字符串比较
来源：http://hz.snrcjt.cn/gtyewkmkjl.html

strcmp(a, b) == 0
来源：http://hz.9152youxi.cn/gtcpkyxtkc.html

[S07] C：数组遍历求和
来源：http://hz.guowangkeji.top/gtngzlvuux.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xylfe.cn/gtdzlwfsfl.html

[S08] C：动态内存分配与释放
来源：http://hz.cashguo.top/gtjryniltw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ydzc1.top/gtsoqvedqw.html

[S09] C：结构体定义与初始化
来源：http://hz.chenjidiqi.icu/gtwqyjvmxq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ivvv.top/gtjlmcknfb.html

[S10] C：指针与解引用
来源：http://hz.birdmap.top/gtafcovnqz.html

int *p = &a;  *p = 5;
来源：http://hz.yj20258.top/gtkywherra.html

[S11] C：逐行读文件
来源：http://hz.hywenlv.cn/gtzobjtrwv.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.aizwys.cn/gtbhsiiusf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.xinyue.icu/gtpzhistqn.html

fclose(f);
来源：http://hz.nwbrower.top/gtujlcanym.html

[S12] C：写文件
来源：http://hz.cdnleiting.top/gtqqisfgaw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.gaohongyu789.top/gtqpmcpspt.html

[S13] C：宏定义
来源：http://hz.sysykeji.top/gtluxcdepq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.bjfxy.top/gtbfdryoay.html

[S14] C：枚举
来源：http://hz.chenlongwang.top/gtraomarao.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.feifeiyinyue.top/gthbeltxmn.html

[S15] C：类型转换
来源：http://hz.daria6918.cn/gtkyvgemze.html

(double) a / b
来源：http://hz.zhixingplan.top/gtegfgjyan.html

[S16] C：位操作置位
来源：http://hz.shzxlz.cn/gtakxbdpmc.html

x |= (1 << 3);
来源：http://hz.yonumen.top/gtaiofvlct.html

[S17] C：安全拼接字符串
来源：http://hz.yuxming.cn/gtukjlfpal.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hammf.cn/gtvqfofkaw.html

[S18] C：命令行参数
来源：http://hz.pengpengdd.cyou/gtqudkyaln.html

int main(int argc, char **argv)
来源：http://hz.zhixingplan.top/gtwwsvpwou.html

[S19] C：快速排序
来源：http://hz.guannengcc.top/gtdzlrqqrq.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cdnleiting.top/gtoiojgjti.html

[S20] C：二分查找
来源：http://hz.ybcxt.top/gtwdgptegk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ehwqpu.com/gtrlzhcrxy.html

[S21] C：字符类别判断
来源：http://hz.meibo888.top/gtzwromrsj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hammf.cn/gtosskuicw.html

[S22] C：字符串转数字
来源：http://hz.jlsjyb.cn/gtfaisudte.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.kuanghao11.cn/gtxbdezkfh.html

[S23] C：随机数
来源：http://hz.gaohongyu789.top/gtbmghytxq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.aizwys.cn/gtmvgxtyyf.html

[S24] C：获取本地时间
来源：http://hz.sysykeji.top/gtbgmtqhdc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhongyouzk.top/gthueuqjnu.html

[S25] C：内存拷贝
来源：http://hz.sysykeji.top/gtjaxxgcuk.html

memcpy(dst, src, n);
来源：http://hz.chenjidiqi.icu/gtpbdjwrsj.html

[S26] C：内存清零
来源：http://hz.bjfxy.top/gtittoypbr.html

memset(a, 0, sizeof a);
来源：http://hz.jinyuanbaomall.cn/gtssqnxkda.html

[S27] C：定义常量
来源：http://hz.zycfv.cn/gtnzvmzshc.html

const double PI = 3.14159;
来源：http://hz.316326.xyz/gtfjpllvjl.html

[S28] C：静态变量
来源：http://hz.yuanzhike.top/gtpithhwva.html

static int counter = 0;
来源：http://hz.jqgufenzy.top/gtlpjpzbwz.html

[S29] C：变参函数
来源：http://hz.shangyingyoupin.top/gtpkbwuoqb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.fzhhl.top/gtbladabyi.html

[S30] C：头文件保护
来源：http://hz.yj20258888.top/gtcvlumkpw.html

#ifndef X_H
来源：http://hz.dianchejie.cn/gtsuslvpls.html

#define X_H
来源：http://hz.shangyingyoupin.top/gtxoqnjstd.html

#endif
来源：http://hz.hammf.cn/gtdeloxjto.html

[S31] C++：Hello World
来源：http://hz.yvedp.cn/gtzgucmdns.html

#include <iostream>
来源：http://hz.tanke756.top/gtpzxvboej.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.daria6918.cn/gtnlegsmdj.html

[S32] C++：字符串
来源：http://hz.hnxiangtu.top/gtpbwokiri.html

std::string s = "hi";  s += "!";
来源：http://hz.chenzaomai.com/gtzgownxnr.html

[S33] C++：vector 增删
来源：http://hz.pycfn.com/gttxfehiru.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.daria6918.cn/gtuijhhmhw.html

[S34] C++：遍历 vector
来源：http://hz.redwolf501.top/gtffnrtnhx.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xziqi.cn/gtepfwqsdd.html

[S35] C++：map
来源：http://hz.snrcjt.cn/gtcpyseqyg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sweek.top/gtndxwfscq.html

[S36] C++：unordered_map
来源：http://hz.yanxiufei.cn/gtjhabozho.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yanxiufei.cn/gtkuvsyjeq.html

[S37] C++：set
来源：http://hz.jqgufenzy.top/gtpwozritc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.nanxuanxn.top/gtwmkrkntn.html

[S38] C++：排序
来源：http://hz.gotoacloud.top/gtfgxhomea.html

std::sort(v.begin(), v.end());
来源：http://hz.yanxiufei.cn/gtjsjmhahr.html

[S39] C++：自定义比较器排序
来源：http://hz.shuidangran.top/gtqgmhqzrb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shangyingyoupin.top/gtjloyueer.html

[S40] C++：查找元素
来源：http://hz.guowangkeji.top/gtytlbueck.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.9152youxi.cn/gtzvclwntl.html

[S41] C++：类与构造函数
来源：http://hz.ehwqpu.com/gtmrpllxrl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhongyouzk.top/gtstoptaqe.html

[S42] C++：继承与虚函数
来源：http://hz.xuanzx.com/gtuweomqry.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhengqikj.top/gtklputqla.html

[S43] C++：智能指针
来源：http://hz.chenzaomai.com/gthxhkryya.html

auto p = std::make_unique<int>(5);
来源：http://hz.yuanzhike.top/gtexvkkvdg.html

[S44] C++：引用传参
来源：http://hz.zhiwuduotai.top/gtlynhdlbv.html

void inc(int &x) { ++x; }
来源：http://hz.fengsongda.top/gtkoromzba.html

[S45] C++：lambda
来源：http://hz.zdqjudy.top/gtozzdsqhm.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.shanyushiyangtech.top/gtxlfxwfdf.html

[S46] C++：函数模板
来源：http://hz.haohaochexian.top/gtvpvbfuyz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.xuanzx.com/gtpaaapawn.html

[S47] C++：结构化绑定遍历
来源：http://hz.pycfn.com/gtiindgnbl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zdqjudy.top/gtezonbrkj.html

[S48] C++：逐行读文件
来源：http://hz.dashuyun.cn/gtoywzppje.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.sxryk.cn/gtebltdsjl.html

while (std::getline(in, line)) { }
来源：http://hz.zhixingplan.top/gthuyhxcdm.html

[S49] C++：写文件
来源：http://hz.zhoulong.xyz/gtuzyfemsk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jqgfzy.top/gttwcjvflm.html

[S50] C++：格式化数字
来源：http://hz.quarkkingdee.top/gthnxupqpv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.daria6918.cn/gtfwthwxmr.html

[S51] C++：显式类型转换
来源：http://hz.pycfn.com/gtirokujlf.html

static_cast<double>(a) / b
来源：http://hz.shangyingyoupin.top/gtfjrecwkh.html

[S52] C++：const 与 noexcept
来源：http://hz.fengsongda.top/gtyyzkwzuv.html

int size() const noexcept { return n_; }
来源：http://hz.ywan-chungtsiang.top/gtfqurykqp.html

[S53] C++：移动语义
来源：http://hz.hnxiangtu.top/gtqfkkcgzd.html

std::vector<int> w = std::move(v);
来源：http://hz.hnxiangtu.top/gtbtonkigw.html

[S54] C++：异常处理
来源：http://hz.yvedp.cn/gtovmstwhc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.sufxvd.cn/gtwzqavatu.html

[S55] C++：结构化绑定
来源：http://hz.feifeiyinyue.top/gtizqltxph.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhiwuduotai.top/gttqxiejno.html

[S56] C++：optional
来源：http://hz.yueranfly.top/gtsofpdadl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hnxiangtu.top/gtygitsdwr.html

[S57] C++：编译期常量
来源：http://hz.hywenlv.cn/gtcxkhqyle.html

constexpr int N = 10;
来源：http://hz.sufxvd.cn/gtfkwxggnt.html

[S58] C++：命名空间
来源：http://hz.yj20258888.top/gtcjvyezep.html

namespace ns { int f() { return 1; } }
来源：http://hz.cqqwz.cn/gtmdwzumbi.html

[S59] C++：静态断言
来源：http://hz.jinqigfzy.top/gtgsulxisa.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sysykeji.top/gtqlncwklv.html

[S60] C++：遍历并删除元素
来源：http://hz.cucudq.cn/gtsdfkvkjs.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hnqzz.top/gthlcygpja.html

================================================================================
来源：http://hz.hywenlv.cn/gtczfchjoq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hywenlv.cn/gtkuryvlwb.html

================================================================================
来源：http://hz.vqdsnc.cn/gtnbvxnwtn.html

[T01] Kotlin：Hello World
来源：http://hz.nanxinkj.top/gtohnhaduk.html

println("Hello")
来源：http://hz.quarkkingdee.top/gtrjsiiwhs.html

[T02] Kotlin：变量
来源：http://hz.shangyingyoupin.top/gtusfhnwhu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xuanzx.com/gtfldaucxi.html

[T03] Kotlin：字符串模板
来源：http://hz.daria6918.cn/gtmwrnlfgp.html

"值: $b"
来源：http://hz.xinyue.icu/gtunrwqzno.html

[T04] Kotlin：空安全
来源：http://hz.iojbl.cn/gtspfcuveg.html

val n: String? = null;  n?.length
来源：http://hz.tian-w.cn/gtsxpsjomp.html

[T05] Kotlin：when 表达式
来源：http://hz.birdmap.top/gtuvvxloxi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.sysykeji.top/gtbgzyvipz.html

[T06] Kotlin：集合映射
来源：http://hz.ehwqpu.com/gtqsfrnwhs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhaomingkeji.xyz/gtwwjjoetk.html

[T07] Kotlin：集合过滤
来源：http://hz.zhijiandao.cn/gtzhiznkif.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jqgufenzy.top/gtumjddjjs.html

[T08] Kotlin：数据类
来源：http://hz.svipenyu.cn/gtumiugehv.html

data class User(val name: String, val age: Int)
来源：http://hz.chenjidiqi.icu/gtrfyumvow.html


<!-- 参考信息 -->