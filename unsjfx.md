代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.quarkkingdee.top/gtyvpnbmdn.html

[R08] 数值比较
来源：http://hz.ybcxt.top/gtjhldbkcy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.haohaochexian.top/gtkjmxjktz.html

[R09] 字符串比较
来源：http://hz.yuxming.cn/gtjnlhtipk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xziqi.cn/gtlvaewwcu.html

[R10] 正则匹配
来源：http://hz.zhixingplan.top/gtmrtqsvhd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.gotoacloud.top/gtszvultnj.html

[R11] case 多分支
来源：http://hz.quarkkingdee.top/gtzvsaodza.html

case "$1" in
来源：http://hz.redwolf501.top/gtlvmehgca.html

start) echo "启动" ;;
来源：http://hz.zhijiandao.cn/gtruedoyki.html

stop)  echo "停止" ;;
来源：http://hz.jinyuanbaomall.cn/gtryvquqvn.html

*)     echo "未知命令" ;;
来源：http://hz.ydjk.org.cn/gtpmdmomgq.html

esac
来源：http://hz.redwolf501.top/gtsmztacoz.html

[R12] for 遍历文件
来源：http://hz.gotoacloud.top/gtebhevkqi.html

for f in *.txt; do echo "$f"; done
来源：http://hz.sxryk.cn/gtziqowwup.html

[R13] for 计数循环
来源：http://hz.chenlongwang.top/gtcfwegpdj.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.pycfn.com/gtduwhgzrc.html

[R14] C 风格 for
来源：http://hz.fzhhl.top/gtfrzsnxrp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yj202588.top/gtdgmafqxf.html

[R15] while 逐行读文件
来源：http://hz.dianchejie.cn/gtejlrqwfx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.nanxuanxn.top/gtalsmkfqf.html

[R16] until 等待条件
来源：http://hz.tian-w.cn/gtqrsifwmq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.xinyue.icu/gtkocsmmqi.html

[R17] 数组定义与取值
来源：http://hz.c1oappe.top/gtbaolnwri.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xinyue.icu/gthgclnfiv.html

[R18] 遍历数组
来源：http://hz.zdqjudy.top/gttjajodib.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shanyushiyangkeji.top/gthsjikyif.html

[R19] 数组长度
来源：http://hz.hammf.cn/gtrnmgxvfv.html

echo "${#arr[@]}"
来源：http://hz.yuxming.cn/gtwnivwifg.html

[R20] 关联数组（字典）
来源：http://hz.hysaishi.cn/gtrkgcckjz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yonumen.top/gtvmxkuhil.html

[R21] 字符串长度
来源：http://hz.hongshengwenyu.top/gtdogwntvf.html

echo "${#s}"
来源：http://hz.jinyuanbaomall.cn/gtiupupgdg.html

[R22] 截取子串
来源：http://hz.hammf.cn/gtnnhbtsiw.html

echo "${s:0:5}"
来源：http://hz.cqqwz.cn/gtjvangypn.html

[R23] 字符串替换
来源：http://hz.smart0.xyz/gtnhxbdory.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.dashuyun.cn/gtnhvglbsd.html

[R24] 大小写转换
来源：http://hz.havefunace.top/gtbnshpebl.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ydzc1.top/gtvyvjvzpy.html

[R25] 去后缀 / 去前缀
来源：http://hz.cqqwz.cn/gtrxgaiabs.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.chenlongwang.top/gtaawizwoj.html

[R26] 命令替换
来源：http://hz.havefunace.top/gthbcaaljn.html

now=$(date +%F); echo "$now"
来源：http://hz.yongpay.top/gtbpvoggjb.html

[R27] 算术展开
来源：http://hz.zhiwuduotai.top/gtrzhtshov.html

echo $((1 + 2 * 3))
来源：http://hz.0kj1m.cn/gtislrhids.html

[R28] 浮点运算
来源：http://hz.fzhhl.top/gtgnxcjbwj.html

echo "scale=2; 10/3" | bc
来源：http://hz.fengsongda.top/gtekgybajj.html

[R29] 定义函数
来源：http://hz.zhoulong.xyz/gtbpfvasgw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.shangyingyoupin.top/gtigjycyty.html

[R30] 函数返回状态码
来源：http://hz.fzhhl.top/gtcxowwdbh.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.daxiang520.top/gtkbbqhwfj.html

[R31] 局部变量
来源：http://hz.shuidangran.top/gtsvnhaaap.html

f() { local x=1; echo "$x"; }
来源：http://hz.xziqi.cn/gtqdtcpbcf.html

[R32] 参数个数校验
来源：http://hz.shuidangran.top/gtatrleecd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.c1oappe.top/gtkijtskqv.html

[R33] 捕获错误并提示行号
来源：http://hz.shanyushiyangkeji.top/gtekvbdtix.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shangyingyoupin.top/gtycxvleca.html

[R34] 退出时清理
来源：http://hz.zhongyouzk.top/gthygerdyf.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.meibo888.top/gtfnadtnkd.html

[R35] 后台执行并等待
来源：http://hz.xziqi.cn/gthoocmpph.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jqgfzy.top/gtiyccwutj.html

[R36] 并发执行多个任务
来源：http://hz.jinghuilouyu.cn/gtivbjtxje.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.vqdsnc.cn/gtocthgpya.html

[R37] 把输出赋给变量
来源：http://hz.shangyingyoupin.top/gtljrhctlo.html

files=$(ls -1)
来源：http://hz.cqqwz.cn/gtmneygqgs.html

[R38] 管道串联
来源：http://hz.shuidangran.top/gtmoskoccr.html

cat a.txt | grep -i error | wc -l
来源：http://hz.mhx1999.top/gtveyhrbos.html

[R39] 重定向标准输出与错误
来源：http://hz.shangyingyoupin.top/gtjuxdtloq.html

cmd > out.log 2>&1
来源：http://hz.jinyuanbaomall.cn/gtiidffknl.html

[R40] 追加写日志
来源：http://hz.cashguo.top/gtrjyautvq.html

echo "log" >> out.log
来源：http://hz.ydjk.org.cn/gtlgfwbwei.html

[R41] 丢弃输出
来源：http://hz.wangdashe.top/gtveonyxwg.html

cmd >/dev/null 2>&1
来源：http://hz.yonumen.top/gtrioahmih.html

[R42] 输入重定向
来源：http://hz.zycfv.cn/gttmlflugg.html

wc -l < a.txt
来源：http://hz.yuanzhike.top/gtzfylymmd.html

[R43] 按名字查找文件
来源：http://hz.xuanzx.com/gtvdgvsxpx.html

find . -name "*.log" -type f
来源：http://hz.shangyingyoupin.top/gtwwsgmesa.html

[R44] 按修改时间查找
来源：http://hz.zhijiandao.cn/gtthjjdgub.html

find . -mtime -7 -type f
来源：http://hz.yj20258888.top/gtextjccjq.html

[R45] 批量删除
来源：http://hz.cdnleiting.top/gtjzevzeax.html

find . -name "*.tmp" -delete
来源：http://hz.nanxuanxn.top/gtojvnjovr.html

[R46] 递归替换文件内容
来源：http://hz.zhoulong.xyz/gtbtkbqklu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.daxiang520.top/gtmfndzdxs.html

[R47] sed 单行替换
来源：http://hz.yongpay.top/gtvzpbrjhe.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yongpay.top/gtstsgfrqm.html

[R48] awk 取指定列
来源：http://hz.nanxinkj.top/gtgubmucjv.html

awk '{print $1, $3}' a.txt
来源：http://hz.yvedp.cn/gtvfagloes.html

[R49] awk 带条件
来源：http://hz.ehwqpu.com/gtdqpbikic.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ywan-chungtsiang.top/gtpmxjwoah.html

[R50] awk 求和
来源：http://hz.bjfxy.top/gtitndacaj.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.quarkkingdee.top/gtxflteoov.html

[R51] 排序去重取前几
来源：http://hz.redwolf501.top/gtdinqpiyp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ehwqpu.com/gtyoytgmns.html

[R52] 统计行数
来源：http://hz.tanke756.top/gttlmyjfdo.html

wc -l a.txt
来源：http://hz.andypj.xyz/gtvayfafst.html

[R53] 查看文件头与实时尾
来源：http://hz.xylfe.cn/gtcpdtuulp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shanyushiyangtech.top/gtrvwayblg.html

[R54] 比较两个文件
来源：http://hz.havefunace.top/gtmjcsoidm.html

diff a.txt b.txt
来源：http://hz.ppjwa.cn/gtrcvtwuqd.html

[R55] 压缩与解压
来源：http://hz.vqdsnc.cn/gtvievfqqk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.fzhhl.top/gtqjhnjolq.html

[R56] 远程拷贝
来源：http://hz.yuanzhike.top/gtkgbydnta.html

scp file user@host:/path/
来源：http://hz.gaohongyu789.top/gtiglrkaco.html

[R57] 远程执行命令
来源：http://hz.yvedp.cn/gtntltmjvr.html

ssh user@host 'uptime'
来源：http://hz.shzxlz.cn/gtfmjpckzv.html

[R58] 下载文件
来源：http://hz.cqqwz.cn/gtvuoiblds.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.cashguo.top/gtygekheet.html

[R59] 发 POST JSON
来源：http://hz.yj202588.top/gtsmbwkeus.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.wangshuangyany.cn/gtkdjbkzxd.html

[R60] 只看 HTTP 状态码
来源：http://hz.cdnleiting.top/gteicoejeb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.shzxlz.cn/gtyibvquou.html

[R61] 磁盘占用
来源：http://hz.jinghuilouyu.cn/gtscsldedj.html

df -h;  du -sh *
来源：http://hz.chenjidiqi.icu/gtbwrromwe.html

[R62] 找最占空间的文件
来源：http://hz.gaohongyu789.top/gtlqeybsbo.html

du -ah . | sort -rh | head -10
来源：http://hz.jqgufenzy.top/gtnhuypayj.html

[R63] 内存与进程
来源：http://hz.0kj1m.cn/gtvmbibtlr.html

free -h;  ps aux | grep nginx
来源：http://hz.wangdashe.top/gtoakypulo.html

[R64] 结束进程
来源：http://hz.xingfuxueyuan.xyz/gtkedezffz.html

kill -9 $(pgrep -f app.py)
来源：http://hz.nwbrower.top/gtdydgacol.html

[R65] 查看端口占用
来源：http://hz.yueranfly.top/gtwwkaohlh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.sufxvd.cn/gtsohjfohp.html

[R66] 定时任务
来源：http://hz.hnxiangtu.top/gtzkuxjtqy.html

crontab -e;  crontab -l
来源：http://hz.jlsjyb.cn/gthkhlakat.html

[R67] 生成随机十六进制串
来源：http://hz.shanyushiyangtech.top/gtlghibpqn.html

openssl rand -hex 16
来源：http://hz.ivvv.top/gtqgjikkxk.html

[R68] 计算文件校验值
来源：http://hz.zhongyouzk.top/gtxgmbzygs.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xingfuxueyuan.xyz/gtilscczxh.html

[R69] 生成随机密码
来源：http://hz.xuanzx.com/gtqgytbpzt.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhijiandao.cn/gtufenzzvi.html

[R70] 时间戳与互转
来源：http://hz.redwolf501.top/gtwldjtqmq.html

date +%s;  date -d @1700000000
来源：http://hz.dianchejie.cn/gtqltmfdoe.html

[R71] 日期格式化
来源：http://hz.xuanzx.com/gtdxaoylic.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.dashuyun.cn/gtsqozouem.html

[R72] 等待端口就绪
来源：http://hz.chenzaomai.com/gtbhvotrvk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.c1oappe.top/gtgkdtnybs.html

[R73] 分割大日志
来源：http://hz.daria6918.cn/gtzmheudlm.html

split -l 1000 big.log part_
来源：http://hz.52xcode.cn/gtofujhvlc.html

[R74] 批量重命名
来源：http://hz.zycfv.cn/gtekmqlkcu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.nanxuanxn.top/gtucmhmrhn.html

[R75] 导出环境变量
来源：http://hz.redwolf501.top/gtdgnqaofi.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.guannengcc.top/gtgrkddydh.html

[R76] 使用临时文件
来源：http://hz.sweek.top/gtqubukyjo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.fengsongda.top/gtocimfifn.html

[R77] 读取用户输入
来源：http://hz.mhx1999.top/gtrfftkddl.html

read -rp "请输入: " ans
来源：http://hz.xinyue.icu/gtffxfqdpf.html

[R78] 交互式菜单
来源：http://hz.smart0.xyz/gtpculgaza.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.gogol.net.cn/gtzzoobmds.html

[R79] 解析命令行选项
来源：http://hz.gzhubu.top/gtdhyvgvxb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.haohaochexian.top/gtzxtidyeh.html

[R80] 查看脚本执行耗时
来源：http://hz.ydjk.org.cn/gtmajvwnya.html

time ./run.sh
来源：http://hz.yangfankeji.com/gtclbstswr.html

================================================================================
来源：http://hz.pengpengdd.cyou/gttkapybaz.html

S. C / C++ 专题
来源：http://hz.pycfn.com/gtvyzchpte.html

================================================================================
来源：http://hz.chenlongwang.top/gtnqkdlbaf.html

[S01] C：Hello World
来源：http://hz.jinqigfzy.top/gtzatqkrfn.html

#include <stdio.h>
来源：http://hz.yj20258888.top/gtpxzudrse.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhongyouzk.top/gtmnwtdbug.html

[S02] C：变量与格式化输出
来源：http://hz.ybcxt.top/gtasgmlrui.html

int a = 10; printf("%d\n", a);
来源：http://hz.9152youxi.cn/gtgsmqshyc.html

[S03] C：读入整数
来源：http://hz.yuxming.cn/gtxswdbxkf.html

int x; scanf("%d", &x);
来源：http://hz.chenjidiqi.icu/gtxpdkvpuw.html

[S04] C：字符串复制
来源：http://hz.ppjwa.cn/gtbigoaafh.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.havefunace.top/gtxtdtqpye.html

[S05] C：字符串长度
来源：http://hz.yj20258888.top/gtltytliic.html

strlen(s)
来源：http://hz.havefunace.top/gtyvikoeuf.html

[S06] C：字符串比较
来源：http://hz.shanyushiyangtech.top/gtqnkitgsm.html

strcmp(a, b) == 0
来源：http://hz.pycfn.com/gtbharmvlk.html

[S07] C：数组遍历求和
来源：http://hz.c1oappe.top/gtriyegsxj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hywenlv.cn/gtxattwjad.html

[S08] C：动态内存分配与释放
来源：http://hz.zhaomingkeji.xyz/gtbgclxxwc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jiagoushi.top/gtcnxtsevp.html

[S09] C：结构体定义与初始化
来源：http://hz.yvedp.cn/gttymqdqcs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jqgfzy.top/gtwfasbekc.html

[S10] C：指针与解引用
来源：http://hz.feifeiyinyue.top/gtkjbikkrz.html

int *p = &a;  *p = 5;
来源：http://hz.xuanzx.com/gtyeqmbrtf.html

[S11] C：逐行读文件
来源：http://hz.ywan-chungtsiang.top/gtluqqgouf.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.hnqzz.top/gtvjgnhbbd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.nanxuanxn.top/gthydqdzch.html

fclose(f);
来源：http://hz.zhoulong.xyz/gtkyatixlc.html

[S12] C：写文件
来源：http://hz.sxryk.cn/gtflhhincg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ywan-chungtsiang.top/gtjnkwhnga.html

[S13] C：宏定义
来源：http://hz.c1oappe.top/gtncnmanwf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.snrcjt.cn/gttlaqakgs.html

[S14] C：枚举
来源：http://hz.hywenlv.cn/gtyzfequla.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yj20258888.top/gtcdantnzz.html

[S15] C：类型转换
来源：http://hz.xuanzx.com/gtucrbmjxd.html

(double) a / b
来源：http://hz.sufxvd.cn/gtvbihdxva.html

[S16] C：位操作置位
来源：http://hz.dianchejie.cn/gtkqhcxtcb.html

x |= (1 << 3);
来源：http://hz.gzhubu.top/gtmcpugnza.html

[S17] C：安全拼接字符串
来源：http://hz.yangfankeji.com/gteezsagvn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.haohaochexian.top/gtcckdqrgb.html

[S18] C：命令行参数
来源：http://hz.yanxiufei.cn/gtfwafkhbe.html

int main(int argc, char **argv)
来源：http://hz.jinghuilouyu.cn/gtpxfcwfop.html

[S19] C：快速排序
来源：http://hz.yuxming.cn/gthxtfnskm.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.pengpengdd.cyou/gtiixvbfuu.html

[S20] C：二分查找
来源：http://hz.zhoulong.xyz/gtaszgqvgl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhaomingkeji.xyz/gtvliitfqw.html

[S21] C：字符类别判断
来源：http://hz.jyoumei.cn/gtbxaqduob.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.snrcjt.cn/gtoqjtwkoi.html

[S22] C：字符串转数字
来源：http://hz.sysykeji.top/gtagqsvhpl.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.nwbrower.top/gtfkdbabwb.html

[S23] C：随机数
来源：http://hz.snrcjt.cn/gtyvgyiwft.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.quarkkingdee.top/gtjljokfmr.html

[S24] C：获取本地时间
来源：http://hz.gaohongyu789.top/gtggedpwzo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.aizwys.cn/gttebecgzn.html

[S25] C：内存拷贝
来源：http://hz.sweek.top/gtazjyukvb.html

memcpy(dst, src, n);
来源：http://hz.chenzaomai.com/gthixdaqdn.html

[S26] C：内存清零
来源：http://hz.kuanghao11.cn/gthkvsfznl.html

memset(a, 0, sizeof a);
来源：http://hz.yongpay.top/gtkdhnodin.html

[S27] C：定义常量
来源：http://hz.quarkkingdee.top/gteykosuie.html

const double PI = 3.14159;
来源：http://hz.xingfuxueyuan.xyz/gturtefdtt.html

[S28] C：静态变量
来源：http://hz.zhongyouzk.top/gtphkefegf.html

static int counter = 0;
来源：http://hz.meibo888.top/gtpnshwbgz.html

[S29] C：变参函数
来源：http://hz.gzhubu.top/gtkxedmgft.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.andypj.xyz/gteckhnokx.html

[S30] C：头文件保护
来源：http://hz.ywan-chungtsiang.top/gtepnyxhjs.html

#ifndef X_H
来源：http://hz.guannengcc.top/gtnbmlncjz.html

#define X_H
来源：http://hz.yonumen.top/gtpbzenotq.html

#endif
来源：http://hz.ydjk.org.cn/gtxbdzwdfa.html

[S31] C++：Hello World
来源：http://hz.hnqzz.top/gtabpfikrx.html

#include <iostream>
来源：http://hz.yj20258.top/gtgdclcwpi.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.cqqwz.cn/gtpxwnssww.html

[S32] C++：字符串
来源：http://hz.snrcjt.cn/gthwgyvpob.html

std::string s = "hi";  s += "!";
来源：http://hz.yj20258888.top/gtulxsznyn.html

[S33] C++：vector 增删
来源：http://hz.vqdsnc.cn/gtvbwshtil.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.aibaodan.cn/gtjayofiyj.html

[S34] C++：遍历 vector
来源：http://hz.zdqjudy.top/gtldjfygxy.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xinyue.icu/gtrzzplzzx.html

[S35] C++：map
来源：http://hz.xuetiantiany.cn/gthbzhkojs.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sxryk.cn/gtdyezgdmq.html

[S36] C++：unordered_map
来源：http://hz.52xcode.cn/gtdepmxmzg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenlongwang.top/gttwjpeybp.html

[S37] C++：set
来源：http://hz.xuanzx.com/gtaxpvoebm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.nanxinkj.top/gtebeoecvk.html

[S38] C++：排序
来源：http://hz.zhixingplan.top/gtzuswahmr.html

std::sort(v.begin(), v.end());
来源：http://hz.cdnleiting.top/gtoufbsquk.html

[S39] C++：自定义比较器排序
来源：http://hz.havefunace.top/gtsfsmviwz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.nwbrower.top/gtbigexbvc.html

[S40] C++：查找元素
来源：http://hz.zhijiandao.cn/gttjcxfyge.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.aibaodan.cn/gtmfefhmbc.html

[S41] C++：类与构造函数
来源：http://hz.hnxiangtu.top/gthdgcppsx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ybcxt.top/gtlemesjjz.html

[S42] C++：继承与虚函数
来源：http://hz.yuanzhike.top/gtrmkfyzbo.html

class B : public Base { public: void f() override {} };
来源：http://hz.wangshuangyany.cn/gthdxjyesr.html

[S43] C++：智能指针
来源：http://hz.vqdsnc.cn/gtnycqygrn.html

auto p = std::make_unique<int>(5);
来源：http://hz.meibo888.top/gthulutftz.html

[S44] C++：引用传参
来源：http://hz.dashuyun.cn/gteijpdinm.html

void inc(int &x) { ++x; }
来源：http://hz.aizwys.cn/gtfwafcthr.html

[S45] C++：lambda
来源：http://hz.wangshuangyany.cn/gttkijtvvf.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hysaishi.cn/gtrgxffney.html

[S46] C++：函数模板
来源：http://hz.nwbrower.top/gtqdeqomnu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.havefunace.top/gtoigbxicc.html

[S47] C++：结构化绑定遍历
来源：http://hz.cucudq.cn/gtnsntirnh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.smart0.xyz/gtnwgeswgp.html

[S48] C++：逐行读文件
来源：http://hz.nanxuanxn.top/gtjwtiwkwa.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.smart0.xyz/gtjrfbzfgi.html

while (std::getline(in, line)) { }
来源：http://hz.aizwys.cn/gtlpdtylup.html

[S49] C++：写文件
来源：http://hz.meibo888.top/gtujdlgjau.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.xinyue.icu/gtalrqamnu.html

[S50] C++：格式化数字
来源：http://hz.c1oappe.top/gtgaxeszzr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jinqigfzy.top/gtsmyuejaw.html

[S51] C++：显式类型转换
来源：http://hz.pengpengdd.cyou/gtmebectds.html

static_cast<double>(a) / b
来源：http://hz.dianchejie.cn/gtzgsnxaaa.html

[S52] C++：const 与 noexcept
来源：http://hz.tian-w.cn/gtxpzbvujh.html

int size() const noexcept { return n_; }
来源：http://hz.birdmap.top/gtlqsjiyto.html

[S53] C++：移动语义
来源：http://hz.andypj.xyz/gtfjbdqwtn.html

std::vector<int> w = std::move(v);
来源：http://hz.zhixingplan.top/gtencgpjny.html

[S54] C++：异常处理
来源：http://hz.ywan-chungtsiang.top/gtgkgtbgvj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xuetiantiany.cn/gtmecgwzao.html

[S55] C++：结构化绑定
来源：http://hz.hysaishi.cn/gtwbugsviu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.tanke756.top/gtttfixzpk.html

[S56] C++：optional
来源：http://hz.zhengqikj.top/gtzwnetnwu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.cheryme.top/gtjbcgphit.html

[S57] C++：编译期常量
来源：http://hz.nwbrower.top/gtuiwnumpa.html

constexpr int N = 10;
来源：http://hz.yj20258.top/gtgrinxyzw.html

[S58] C++：命名空间
来源：http://hz.mhx1999.top/gtahithdaz.html

namespace ns { int f() { return 1; } }
来源：http://hz.havefunace.top/gtjhqznwnf.html

[S59] C++：静态断言
来源：http://hz.tianlin.xyz/gtglfejlmy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ivvv.top/gtgzbjpbto.html

[S60] C++：遍历并删除元素
来源：http://hz.haohaochexian.top/gtpajckzit.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.tianlin.xyz/gtlnmqjkxk.html

================================================================================
来源：http://hz.mhx1999.top/gtghkmxahu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jiagoushi.top/gtketoqpsf.html

================================================================================
来源：http://hz.ydzc1.top/gtsmgwfzvg.html

[T01] Kotlin：Hello World
来源：http://hz.9152youxi.cn/gtcqwnyvep.html

println("Hello")
来源：http://hz.sufxvd.cn/gtllwzrwlc.html

[T02] Kotlin：变量
来源：http://hz.gzhubu.top/gtjicmbcpa.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yangfankeji.com/gtsmkrsxgb.html

[T03] Kotlin：字符串模板
来源：http://hz.xinyue.icu/gtrrmlzete.html

"值: $b"
来源：http://hz.jinghuilouyu.cn/gtabdfauyz.html

[T04] Kotlin：空安全
来源：http://hz.cucudq.cn/gtnapvkyen.html

val n: String? = null;  n?.length
来源：http://hz.zhixingplan.top/gtvccanegk.html

[T05] Kotlin：when 表达式
来源：http://hz.snrcjt.cn/gtxnksxcvd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.tanke756.top/gtpjndowpc.html

[T06] Kotlin：集合映射
来源：http://hz.zhixingplan.top/gtgnvcagwl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.xylfe.cn/gtuinvrvvq.html

[T07] Kotlin：集合过滤
来源：http://hz.gotoacloud.top/gtfuetomzf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xziqi.cn/gtvqxgpnxu.html

[T08] Kotlin：数据类
来源：http://hz.yonumen.top/gtqocxnufx.html

data class User(val name: String, val age: Int)
来源：http://hz.yangfankeji.com/gtdynmwlth.html


<!-- 参考信息 -->