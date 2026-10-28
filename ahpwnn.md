代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hfpthk.cn/gtwyeguzfd.html

[Q90] 生成序号列
来源：http://hz.xziqi.cn/gtwoujilyq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xylfe.cn/gttgidbsre.html

================================================================================
来源：http://hz.fengsongda.top/gtcnyraydj.html

R. Bash 专题
来源：http://hz.0kj1m.cn/gteyjiwbjx.html

================================================================================
来源：http://hz.hysaishi.cn/gtpfsnysns.html

[R01] shebang 与严格模式
来源：http://hz.xylfe.cn/gtuhahutkv.html

#!/usr/bin/env bash
来源：http://hz.ppjwa.cn/gtqhvbafzh.html

set -euo pipefail
来源：http://hz.gaohongyu789.top/gtvoqryfmd.html

[R02] 变量赋值与使用
来源：http://hz.fengsongda.top/gtifupbjjd.html

name="Tom"; echo "$name"
来源：http://hz.shangyingyoupin.top/gthafaqngn.html

[R03] 只读变量
来源：http://hz.yongpay.top/gtncgrmuny.html

readonly PI=3.14
来源：http://hz.birdmap.top/gtnhryrpzm.html

[R04] 位置参数
来源：http://hz.andypj.xyz/gthxmekrnh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.shzxlz.cn/gtadmbivbl.html

[R05] 参数默认值
来源：http://hz.xingfuxueyuan.xyz/gttmvehjzn.html

name="${1:-default}"
来源：http://hz.jinyuanbaomall.cn/gtftctdofw.html

[R06] 判断命令是否存在
来源：http://hz.jyoumei.cn/gtfhjxihsx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ehwqpu.com/gtmxfebaib.html

[R07] if 判断文件
来源：http://hz.havefunace.top/gtgvyeinfx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jyoumei.cn/gtwvdkajai.html

[R08] 数值比较
来源：http://hz.gaohongyu789.top/gtdajqlzzk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.svipenyu.cn/gttnnwmmtz.html

[R09] 字符串比较
来源：http://hz.cucudq.cn/gtjqwzrhli.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hnqzz.top/gtoijpeubf.html

[R10] 正则匹配
来源：http://hz.tian-w.cn/gtksudlfqb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.sysykeji.top/gtwgfuwyrj.html

[R11] case 多分支
来源：http://hz.xingfuxueyuan.xyz/gthdagfbdy.html

case "$1" in
来源：http://hz.gzhubu.top/gtheoltkmt.html

start) echo "启动" ;;
来源：http://hz.nanxinkj.top/gtadvynrfz.html

stop)  echo "停止" ;;
来源：http://hz.jinqigufen.top/gtmhxjnmfd.html

*)     echo "未知命令" ;;
来源：http://hz.ydzc1.top/gtyuuzitqr.html

esac
来源：http://hz.sufxvd.cn/gthllqhncu.html

[R12] for 遍历文件
来源：http://hz.ivvv.top/gtqczxgrto.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhoulong.xyz/gtbivyrnax.html

[R13] for 计数循环
来源：http://hz.fengsongda.top/gtksmdgkyi.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhijiandao.cn/gtmiuofbtq.html

[R14] C 风格 for
来源：http://hz.tian-w.cn/gtymcsleqw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cashguo.top/gtkohrxnee.html

[R15] while 逐行读文件
来源：http://hz.kuanghao11.cn/gteqedlgtj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.bjfxy.top/gtvjlnuumw.html

[R16] until 等待条件
来源：http://hz.zhixingplan.top/gtfxvtynfh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.chenjidiqi.icu/gtukwvxcvb.html

[R17] 数组定义与取值
来源：http://hz.0kj1m.cn/gtqnirkdgy.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zdqjudy.top/gtirpipkhl.html

[R18] 遍历数组
来源：http://hz.fengsongda.top/gtofynapxp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cqqwz.cn/gtlvxwmoet.html

[R19] 数组长度
来源：http://hz.daxiang520.top/gtisjolzie.html

echo "${#arr[@]}"
来源：http://hz.yj20258.top/gtnxteiyro.html

[R20] 关联数组（字典）
来源：http://hz.redwolf501.top/gtqhoxkgyv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.nanxinkj.top/gtseqbnczh.html

[R21] 字符串长度
来源：http://hz.yvedp.cn/gtbgeauktn.html

echo "${#s}"
来源：http://hz.yvedp.cn/gtauphqjao.html

[R22] 截取子串
来源：http://hz.snrcjt.cn/gtbdwimkba.html

echo "${s:0:5}"
来源：http://hz.ybcxt.top/gtiozrpebb.html

[R23] 字符串替换
来源：http://hz.gaohongyu789.top/gtpkyvhruk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yongpay.top/gtoujnhhms.html

[R24] 大小写转换
来源：http://hz.zhaomingkeji.xyz/gtvsjpomur.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.c1oappe.top/gtbfmiitgn.html

[R25] 去后缀 / 去前缀
来源：http://hz.hywenlv.cn/gtdmkooelj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhongyouzk.top/gtkjswyfli.html

[R26] 命令替换
来源：http://hz.ydzc1.top/gtitaffhpj.html

now=$(date +%F); echo "$now"
来源：http://hz.hammf.cn/gtcpjelglh.html

[R27] 算术展开
来源：http://hz.feifeiyinyue.top/gtwkkmhjcz.html

echo $((1 + 2 * 3))
来源：http://hz.daria6918.cn/gtxxcriybr.html

[R28] 浮点运算
来源：http://hz.zdqjudy.top/gtktdmtypp.html

echo "scale=2; 10/3" | bc
来源：http://hz.quarkkingdee.top/gtlnftxzvs.html

[R29] 定义函数
来源：http://hz.jinyuanbaomall.cn/gtmdrandxv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.fengsongda.top/gtwuctorzb.html

[R30] 函数返回状态码
来源：http://hz.guannengcc.top/gtwtccgkiu.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ppjwa.cn/gtwmngmwld.html

[R31] 局部变量
来源：http://hz.tianlin.xyz/gthvrgpyuc.html

f() { local x=1; echo "$x"; }
来源：http://hz.ydzc1.top/gtyfttkomz.html

[R32] 参数个数校验
来源：http://hz.xziqi.cn/gtcphoeomc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.fengsongda.top/gtngovilvr.html

[R33] 捕获错误并提示行号
来源：http://hz.redwolf501.top/gtbdrakxzv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xuanzx.com/gtnycnxcfq.html

[R34] 退出时清理
来源：http://hz.zdqjudy.top/gtyfdxiscc.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hnxiangtu.top/gttivwtomq.html

[R35] 后台执行并等待
来源：http://hz.xziqi.cn/gtmkrivyua.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.nwbrower.top/gtttulunhb.html

[R36] 并发执行多个任务
来源：http://hz.zycfv.cn/gtbbbqjrwi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.tian-w.cn/gtvynfbiec.html

[R37] 把输出赋给变量
来源：http://hz.meibo888.top/gtdfmcivpn.html

files=$(ls -1)
来源：http://hz.zhoulong.xyz/gtzevrhcsr.html

[R38] 管道串联
来源：http://hz.feifeiyinyue.top/gtodvjkvck.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ywan-chungtsiang.top/gtvfzzygyf.html

[R39] 重定向标准输出与错误
来源：http://hz.nanxuanxn.top/gtbvhpunra.html

cmd > out.log 2>&1
来源：http://hz.quarkkingdee.top/gtynoexrhx.html

[R40] 追加写日志
来源：http://hz.zhoulong.xyz/gtslfwtide.html

echo "log" >> out.log
来源：http://hz.kuanghao11.cn/gtoedjkima.html

[R41] 丢弃输出
来源：http://hz.zhijiandao.cn/gtxhliluqw.html

cmd >/dev/null 2>&1
来源：http://hz.xuanzx.com/gttfeemdkd.html

[R42] 输入重定向
来源：http://hz.smart0.xyz/gtyzlhtfvj.html

wc -l < a.txt
来源：http://hz.snrcjt.cn/gtnupqoqgi.html

[R43] 按名字查找文件
来源：http://hz.ehwqpu.com/gterqwstte.html

find . -name "*.log" -type f
来源：http://hz.shzxlz.cn/gtuojasole.html

[R44] 按修改时间查找
来源：http://hz.ydjk.org.cn/gtehappyeh.html

find . -mtime -7 -type f
来源：http://hz.aizwys.cn/gtnikekysv.html

[R45] 批量删除
来源：http://hz.cheryme.top/gtiakyrqrj.html

find . -name "*.tmp" -delete
来源：http://hz.mhx1999.top/gtqgecaqjj.html

[R46] 递归替换文件内容
来源：http://hz.316326.xyz/gtdixkoziv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yangfankeji.com/gtlkbzivxp.html

[R47] sed 单行替换
来源：http://hz.zhengqikj.top/gtfafbbcvh.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.guannengcc.top/gtuibgtgwy.html

[R48] awk 取指定列
来源：http://hz.wangshuangyany.cn/gtjwjpvxhq.html

awk '{print $1, $3}' a.txt
来源：http://hz.hysaishi.cn/gtmlmlruwa.html

[R49] awk 带条件
来源：http://hz.yvedp.cn/gtoarqyaxk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jyoumei.cn/gtpwomdpuf.html

[R50] awk 求和
来源：http://hz.chenlongwang.top/gtsmxgjjen.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.gogol.net.cn/gtaupkuvwg.html

[R51] 排序去重取前几
来源：http://hz.hnqzz.top/gtjnhghdil.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jiagoushi.top/gtduiskgqi.html

[R52] 统计行数
来源：http://hz.tianlin.xyz/gtggvhxxfv.html

wc -l a.txt
来源：http://hz.9152youxi.cn/gtncalrexl.html

[R53] 查看文件头与实时尾
来源：http://hz.yj20258.top/gtxxsdfslg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.gzhubu.top/gtoxbmoeim.html

[R54] 比较两个文件
来源：http://hz.meibo888.top/gtnytzttdw.html

diff a.txt b.txt
来源：http://hz.fengsongda.top/gtxetudasx.html

[R55] 压缩与解压
来源：http://hz.pycfn.com/gtjfxjquzg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hnxiangtu.top/gtcpatazil.html

[R56] 远程拷贝
来源：http://hz.gogol.net.cn/gtbtueltse.html

scp file user@host:/path/
来源：http://hz.cucudq.cn/gtxyjbzuwz.html

[R57] 远程执行命令
来源：http://hz.hfpthk.cn/gtqtfwqxru.html

ssh user@host 'uptime'
来源：http://hz.jqgfzy.top/gtqlbzdtrs.html

[R58] 下载文件
来源：http://hz.ehwqpu.com/gtjzouhabd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.sweek.top/gtozmnvdof.html

[R59] 发 POST JSON
来源：http://hz.9152youxi.cn/gtytdttjyl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.gotoacloud.top/gtxsuciyje.html

[R60] 只看 HTTP 状态码
来源：http://hz.guowangkeji.top/gtjjukoydm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hammf.cn/gtoewldhbe.html

[R61] 磁盘占用
来源：http://hz.jinyuanbaomall.cn/gtuyaukewz.html

df -h;  du -sh *
来源：http://hz.birdmap.top/gtektmuqxy.html

[R62] 找最占空间的文件
来源：http://hz.zhoulong.xyz/gtnrereawm.html

du -ah . | sort -rh | head -10
来源：http://hz.bjfxy.top/gtztfsphbj.html

[R63] 内存与进程
来源：http://hz.yj20258888.top/gtfrxjrqqt.html

free -h;  ps aux | grep nginx
来源：http://hz.daria6918.cn/gtrirnevbo.html

[R64] 结束进程
来源：http://hz.ydzc1.top/gtewdrlbdg.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hammf.cn/gtczknyebp.html

[R65] 查看端口占用
来源：http://hz.xinyue.icu/gtuqsjwkjr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.kuanghao11.cn/gtweiwgadc.html

[R66] 定时任务
来源：http://hz.nanxinkj.top/gtxfhqspdz.html

crontab -e;  crontab -l
来源：http://hz.tianlin.xyz/gtzgoptndw.html

[R67] 生成随机十六进制串
来源：http://hz.jyoumei.cn/gtysjyrndc.html

openssl rand -hex 16
来源：http://hz.jqgufenzy.top/gtuaeqdqaa.html

[R68] 计算文件校验值
来源：http://hz.xuetiantiany.cn/gtmgwxqyfz.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.haohaochexian.top/gtzzsjlmsq.html

[R69] 生成随机密码
来源：http://hz.smart0.xyz/gtuazhnnzn.html

head -c 16 /dev/urandom | base64
来源：http://hz.hfpthk.cn/gtauvpeelr.html

[R70] 时间戳与互转
来源：http://hz.aizwys.cn/gtrzjnjndw.html

date +%s;  date -d @1700000000
来源：http://hz.zycfv.cn/gtjroxrndx.html

[R71] 日期格式化
来源：http://hz.hnqzz.top/gthaqjbtxv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.c1oappe.top/gtlkjpfkqs.html

[R72] 等待端口就绪
来源：http://hz.gzhubu.top/gttlnynutq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.snrcjt.cn/gtueqqhmoa.html

[R73] 分割大日志
来源：http://hz.xuanzx.com/gtfxppyvse.html

split -l 1000 big.log part_
来源：http://hz.aizwys.cn/gtadatfyid.html

[R74] 批量重命名
来源：http://hz.dashuyun.cn/gtfqsamjrj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.sufxvd.cn/gtufexfiau.html

[R75] 导出环境变量
来源：http://hz.nanxinkj.top/gtddmxgboa.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.haohaochexian.top/gtidkexycy.html

[R76] 使用临时文件
来源：http://hz.haohaochexian.top/gthvhaforc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yongpay.top/gtoiotmhix.html

[R77] 读取用户输入
来源：http://hz.daria6918.cn/gtqviplvks.html

read -rp "请输入: " ans
来源：http://hz.tianlin.xyz/gthstidsii.html

[R78] 交互式菜单
来源：http://hz.daria6918.cn/gtlsaejzmb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.nanxinkj.top/gtqkxcrtwp.html

[R79] 解析命令行选项
来源：http://hz.chenzaomai.com/gtpnotzraq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.birdmap.top/gtztxagrvt.html

[R80] 查看脚本执行耗时
来源：http://hz.zhaomingkeji.xyz/gtxmbefhja.html

time ./run.sh
来源：http://hz.sxryk.cn/gtdnkfnlvd.html

================================================================================
来源：http://hz.fzhhl.top/gtxousfvhr.html

S. C / C++ 专题
来源：http://hz.vqdsnc.cn/gtqxwnwihh.html

================================================================================
来源：http://hz.nanxinkj.top/gtytvpnixk.html

[S01] C：Hello World
来源：http://hz.bjfxy.top/gtnchffmre.html

#include <stdio.h>
来源：http://hz.mhx1999.top/gtyvnlgiko.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jinyuanbaomall.cn/gtldrhmhyo.html

[S02] C：变量与格式化输出
来源：http://hz.gogol.net.cn/gtblsmctxg.html

int a = 10; printf("%d\n", a);
来源：http://hz.yongpay.top/gtybkrtvne.html

[S03] C：读入整数
来源：http://hz.yvedp.cn/gtxnexkwso.html

int x; scanf("%d", &x);
来源：http://hz.kuanghao11.cn/gtzvkujgyd.html

[S04] C：字符串复制
来源：http://hz.ppjwa.cn/gthjudpbmy.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.bjfxy.top/gtuxaszubb.html

[S05] C：字符串长度
来源：http://hz.zdqjudy.top/gtjlwnqulg.html

strlen(s)
来源：http://hz.9152youxi.cn/gtggacnatk.html

[S06] C：字符串比较
来源：http://hz.xylfe.cn/gtiffvusku.html

strcmp(a, b) == 0
来源：http://hz.zhengqikj.top/gtjjglvkcs.html

[S07] C：数组遍历求和
来源：http://hz.yanxiufei.cn/gttgjzhuhk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yangfankeji.com/gtbhmskdcc.html

[S08] C：动态内存分配与释放
来源：http://hz.bjfxy.top/gtihrbydib.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.birdmap.top/gtgnjtneff.html

[S09] C：结构体定义与初始化
来源：http://hz.jyoumei.cn/gtfshcicwa.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.cheryme.top/gtaqzwkbhf.html

[S10] C：指针与解引用
来源：http://hz.ydjk.org.cn/gtshvgqcjz.html

int *p = &a;  *p = 5;
来源：http://hz.ydzc1.top/gthqjruvux.html

[S11] C：逐行读文件
来源：http://hz.ydzc1.top/gtjudmfkyg.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.dashuyun.cn/gtmiqcdxpy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.gogol.net.cn/gtgymfaqzs.html

fclose(f);
来源：http://hz.daria6918.cn/gtymjmjkof.html

[S12] C：写文件
来源：http://hz.guannengcc.top/gtytnzykdy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.kuanghao11.cn/gtnshvcekx.html

[S13] C：宏定义
来源：http://hz.zycfv.cn/gtagruqvaf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.guowangkeji.top/gthnndmkgj.html

[S14] C：枚举
来源：http://hz.tian-w.cn/gtzwxmvfdh.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ydjk.org.cn/gtkullsdma.html

[S15] C：类型转换
来源：http://hz.hysaishi.cn/gtzikccuex.html

(double) a / b
来源：http://hz.vqdsnc.cn/gtfvwqqfku.html

[S16] C：位操作置位
来源：http://hz.tian-w.cn/gtciiffgmf.html

x |= (1 << 3);
来源：http://hz.chenjidiqi.icu/gtlgpcklfa.html

[S17] C：安全拼接字符串
来源：http://hz.feifeiyinyue.top/gtdmhkhjit.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.vqdsnc.cn/gthexqsprj.html

[S18] C：命令行参数
来源：http://hz.mhx1999.top/gtkqdwupul.html

int main(int argc, char **argv)
来源：http://hz.fzhhl.top/gtdrdkfozb.html

[S19] C：快速排序
来源：http://hz.dashuyun.cn/gteurhfkgk.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.52xcode.cn/gtuvtucnpw.html

[S20] C：二分查找
来源：http://hz.yonumen.top/gtmkddxmku.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hywenlv.cn/gtxxtzhqvl.html

[S21] C：字符类别判断
来源：http://hz.zycfv.cn/gtcwbxhkqp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ehwqpu.com/gtiaibfita.html

[S22] C：字符串转数字
来源：http://hz.nanxuanxn.top/gtwgyatxzq.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ydjk.org.cn/gtaemsucee.html

[S23] C：随机数
来源：http://hz.vqdsnc.cn/gtmbhcerff.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.andypj.xyz/gtvlsyvkoq.html

[S24] C：获取本地时间
来源：http://hz.wangshuangyany.cn/gtaryzqybo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.kuanghao11.cn/gtpevzzinm.html

[S25] C：内存拷贝
来源：http://hz.gzhubu.top/gtlcrzjgtm.html

memcpy(dst, src, n);
来源：http://hz.jinqigufen.top/gtcfquftrk.html

[S26] C：内存清零
来源：http://hz.wangshuangyany.cn/gtsncvspjz.html

memset(a, 0, sizeof a);
来源：http://hz.yueranfly.top/gtbbmnobfy.html

[S27] C：定义常量
来源：http://hz.xylfe.cn/gtfirxfftm.html

const double PI = 3.14159;
来源：http://hz.shzxlz.cn/gtjzupwxib.html

[S28] C：静态变量
来源：http://hz.shuidangran.top/gtmedmnoim.html

static int counter = 0;
来源：http://hz.shzxlz.cn/gtzgttqgoh.html

[S29] C：变参函数
来源：http://hz.smart0.xyz/gtekthxoll.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.chenzaomai.com/gtciyvjppp.html

[S30] C：头文件保护
来源：http://hz.52xcode.cn/gtfptzcjon.html

#ifndef X_H
来源：http://hz.sxryk.cn/gtpvrtocgd.html

#define X_H
来源：http://hz.feifeiyinyue.top/gtgxqrleuj.html

#endif
来源：http://hz.zdqjudy.top/gthnzdywic.html

[S31] C++：Hello World
来源：http://hz.yvedp.cn/gtngsvpljm.html

#include <iostream>
来源：http://hz.ywan-chungtsiang.top/gtamgisilz.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.daxiang520.top/gtfsndacem.html

[S32] C++：字符串
来源：http://hz.nwbrower.top/gtnslqxspf.html

std::string s = "hi";  s += "!";
来源：http://hz.hnqzz.top/gtxftzmvik.html

[S33] C++：vector 增删
来源：http://hz.zhixingplan.top/gtgkqzgjqg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xinyue.icu/gtxetyaizb.html

[S34] C++：遍历 vector
来源：http://hz.yvedp.cn/gtzesfkoqe.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.guannengcc.top/gtrqgrqivq.html

[S35] C++：map
来源：http://hz.andypj.xyz/gtupmhlmsq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.birdmap.top/gtleinwgze.html

[S36] C++：unordered_map
来源：http://hz.gzhubu.top/gtggxntgoy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xinyue.icu/gtmrsqfhhr.html

[S37] C++：set
来源：http://hz.yj20258.top/gtdjbztqal.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ydzc1.top/gtdoidjuck.html

[S38] C++：排序
来源：http://hz.wangdashe.top/gtugbrxfbv.html

std::sort(v.begin(), v.end());
来源：http://hz.smart0.xyz/gtiukdvuec.html

[S39] C++：自定义比较器排序
来源：http://hz.shanyushiyangkeji.top/gteoytrcji.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhixingplan.top/gtjbgwirlj.html

[S40] C++：查找元素
来源：http://hz.gaohongyu789.top/gtxnggfybr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ydjk.org.cn/gthjyliggj.html

[S41] C++：类与构造函数
来源：http://hz.yanxiufei.cn/gtkekgrdnv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.sufxvd.cn/gtfxjmamct.html

[S42] C++：继承与虚函数
来源：http://hz.hfpthk.cn/gtrxiabnaj.html

class B : public Base { public: void f() override {} };
来源：http://hz.redwolf501.top/gtlnljovyu.html

[S43] C++：智能指针
来源：http://hz.xziqi.cn/gtfexoddvi.html

auto p = std::make_unique<int>(5);
来源：http://hz.yangfankeji.com/gtenriskid.html

[S44] C++：引用传参
来源：http://hz.tanke756.top/gtfgkzyagm.html

void inc(int &x) { ++x; }
来源：http://hz.nanxuanxn.top/gteenssvnp.html

[S45] C++：lambda
来源：http://hz.wangdashe.top/gtkthmbxpj.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhaomingkeji.xyz/gtjgpcyluk.html

[S46] C++：函数模板
来源：http://hz.gotoacloud.top/gtbugcvsuq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.fengsongda.top/gtimgkptoc.html

[S47] C++：结构化绑定遍历
来源：http://hz.shzxlz.cn/gtubugkjpj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jyoumei.cn/gtesmvmxxy.html

[S48] C++：逐行读文件
来源：http://hz.316326.xyz/gttntdfryv.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.chenjidiqi.icu/gtyxuhqnbd.html

while (std::getline(in, line)) { }
来源：http://hz.sweek.top/gtsrgiidia.html

[S49] C++：写文件
来源：http://hz.ppjwa.cn/gtjmfpwdgz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.fengsongda.top/gtvtewjzaf.html

[S50] C++：格式化数字
来源：http://hz.yonumen.top/gtlxphbohr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.meibo888.top/gtdnylrnyr.html

[S51] C++：显式类型转换
来源：http://hz.cashguo.top/gtfdyuxaju.html

static_cast<double>(a) / b
来源：http://hz.jinghuilouyu.cn/gtafujpvwh.html

[S52] C++：const 与 noexcept
来源：http://hz.ivvv.top/gtvznqqitz.html

int size() const noexcept { return n_; }
来源：http://hz.tian-w.cn/gtxwuflhej.html

[S53] C++：移动语义
来源：http://hz.shzxlz.cn/gtmtkuwmrr.html

std::vector<int> w = std::move(v);
来源：http://hz.cdnleiting.top/gtmhskfbzy.html

[S54] C++：异常处理
来源：http://hz.pycfn.com/gtxxfftgez.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.0kj1m.cn/gtungpnmbm.html

[S55] C++：结构化绑定
来源：http://hz.nanxuanxn.top/gtjzjejmqd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.sufxvd.cn/gtuvxgfagm.html

[S56] C++：optional
来源：http://hz.jqgufenzy.top/gtjvcbqdym.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.birdmap.top/gtaljwojyo.html

[S57] C++：编译期常量
来源：http://hz.zhongyouzk.top/gthsxazizd.html

constexpr int N = 10;
来源：http://hz.aibaodan.cn/gtfyybhojf.html

[S58] C++：命名空间
来源：http://hz.sufxvd.cn/gtpowisktq.html

namespace ns { int f() { return 1; } }
来源：http://hz.pengpengdd.cyou/gtcaevcqkr.html

[S59] C++：静态断言
来源：http://hz.dashuyun.cn/gtvemtvesi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zdqjudy.top/gtgfemynam.html

[S60] C++：遍历并删除元素
来源：http://hz.yanxiufei.cn/gtaacfwlhp.html


<!-- 参考信息 -->