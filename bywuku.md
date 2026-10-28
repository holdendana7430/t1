代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://hz.pengpengdd.cyou/gtephfbwtq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhixingplan.top/gtqaikhvrg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yvedp.cn/gtayxjjvcz.html

[Q89] 判断表是否存在
来源：http://hz.chenlongwang.top/gtgwfbzatf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.sweek.top/gtvpdiaonb.html

[Q90] 生成序号列
来源：http://hz.yvedp.cn/gtuskrsvkt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xziqi.cn/gtpbzohhbq.html

================================================================================
来源：http://hz.gotoacloud.top/gtngepziyg.html

R. Bash 专题
来源：http://hz.xingfuxueyuan.xyz/gtpsfqyhnp.html

================================================================================
来源：http://hz.yongpay.top/gtdsjdlbuh.html

[R01] shebang 与严格模式
来源：http://hz.fzhhl.top/gtwjyagzze.html

#!/usr/bin/env bash
来源：http://hz.meibo888.top/gtejfuljoa.html

set -euo pipefail
来源：http://hz.ydjk.org.cn/gtmrqxpfrt.html

[R02] 变量赋值与使用
来源：http://hz.xinyue.icu/gthrykcbww.html

name="Tom"; echo "$name"
来源：http://hz.gogol.net.cn/gtaxdeesob.html

[R03] 只读变量
来源：http://hz.zhaomingkeji.xyz/gtncuugkyh.html

readonly PI=3.14
来源：http://hz.yj20258888.top/gtrebgfjxi.html

[R04] 位置参数
来源：http://hz.aizwys.cn/gtcngohmgv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cqqwz.cn/gtxhjbdmzv.html

[R05] 参数默认值
来源：http://hz.zhixingplan.top/gthmltonsu.html

name="${1:-default}"
来源：http://hz.yonumen.top/gtngeblsam.html

[R06] 判断命令是否存在
来源：http://hz.ydzc1.top/gtvmzpmznr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.gaohongyu789.top/gtcblrlope.html

[R07] if 判断文件
来源：http://hz.daxiang520.top/gtqlxcmzje.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xziqi.cn/gtoojrpexv.html

[R08] 数值比较
来源：http://hz.chenjidiqi.icu/gtrcayxkwj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.nanxuanxn.top/gtybhbajcd.html

[R09] 字符串比较
来源：http://hz.hammf.cn/gtstsqohll.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.cqqwz.cn/gtjftgagje.html

[R10] 正则匹配
来源：http://hz.feifeiyinyue.top/gtrrcpmofp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.redwolf501.top/gtkmokxaqz.html

[R11] case 多分支
来源：http://hz.hnqzz.top/gtzrmgiuhd.html

case "$1" in
来源：http://hz.cqqwz.cn/gtdwlrpadq.html

start) echo "启动" ;;
来源：http://hz.birdmap.top/gtfutaltyv.html

stop)  echo "停止" ;;
来源：http://hz.zhoulong.xyz/gtvhnhpdxb.html

*)     echo "未知命令" ;;
来源：http://hz.ppjwa.cn/gtzeprahbo.html

esac
来源：http://hz.shuidangran.top/gtlviwqddc.html

[R12] for 遍历文件
来源：http://hz.zycfv.cn/gtjhfsultl.html

for f in *.txt; do echo "$f"; done
来源：http://hz.svipenyu.cn/gthnwmpriw.html

[R13] for 计数循环
来源：http://hz.shuidangran.top/gtyjsctncg.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yueranfly.top/gtlkikkkyd.html

[R14] C 风格 for
来源：http://hz.316326.xyz/gtlvrsimwr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ppjwa.cn/gtjkyyepze.html

[R15] while 逐行读文件
来源：http://hz.shzxlz.cn/gtswocrzgw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zhiwuduotai.top/gtdqmpazlr.html

[R16] until 等待条件
来源：http://hz.chenzaomai.com/gtliarhtst.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhengqikj.top/gtgdxsgauz.html

[R17] 数组定义与取值
来源：http://hz.birdmap.top/gtrlrhgygy.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.quarkkingdee.top/gtunzbagui.html

[R18] 遍历数组
来源：http://hz.meibo888.top/gtkqilzuoc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.guowangkeji.top/gtdmnteqtj.html

[R19] 数组长度
来源：http://hz.xingfuxueyuan.xyz/gtumdjzdce.html

echo "${#arr[@]}"
来源：http://hz.haohaochexian.top/gtecmqzojt.html

[R20] 关联数组（字典）
来源：http://hz.jinghuilouyu.cn/gtwyovgrje.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.tanke756.top/gtptlrvlgf.html

[R21] 字符串长度
来源：http://hz.hammf.cn/gtaynbwvje.html

echo "${#s}"
来源：http://hz.sweek.top/gtcshjowel.html

[R22] 截取子串
来源：http://hz.jyoumei.cn/gtcurymmrt.html

echo "${s:0:5}"
来源：http://hz.hongshengwenyu.top/gtcynrccmp.html

[R23] 字符串替换
来源：http://hz.redwolf501.top/gtundtudka.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ybcxt.top/gtcfxknize.html

[R24] 大小写转换
来源：http://hz.zhiwuduotai.top/gtpzdmsrxl.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.tianlin.xyz/gtunqpumnb.html

[R25] 去后缀 / 去前缀
来源：http://hz.ywan-chungtsiang.top/gtvzpnlsnn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ybcxt.top/gtxkhoigdt.html

[R26] 命令替换
来源：http://hz.jyoumei.cn/gtvuhakhej.html

now=$(date +%F); echo "$now"
来源：http://hz.zdqjudy.top/gtbxfeuhsx.html

[R27] 算术展开
来源：http://hz.hongshengwenyu.top/gtgpixhien.html

echo $((1 + 2 * 3))
来源：http://hz.shanyushiyangkeji.top/gtfapwnpjd.html

[R28] 浮点运算
来源：http://hz.yvedp.cn/gtkschjjul.html

echo "scale=2; 10/3" | bc
来源：http://hz.cucudq.cn/gtniruwjki.html

[R29] 定义函数
来源：http://hz.hfpthk.cn/gttsmllpul.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.wangdashe.top/gtwpfifjzy.html

[R30] 函数返回状态码
来源：http://hz.yj20258888.top/gtjrnebkvn.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xingfuxueyuan.xyz/gttmncsxsl.html

[R31] 局部变量
来源：http://hz.xuetiantiany.cn/gtgtzpafgr.html

f() { local x=1; echo "$x"; }
来源：http://hz.dianchejie.cn/gtincmyuuj.html

[R32] 参数个数校验
来源：http://hz.hnxiangtu.top/gtjmiqiesn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.wangshuangyany.cn/gtxqiyutzh.html

[R33] 捕获错误并提示行号
来源：http://hz.yj20258.top/gtrrimebvi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shuidangran.top/gtvxcyefsc.html

[R34] 退出时清理
来源：http://hz.xziqi.cn/gtslkknstj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.birdmap.top/gtozeyfldr.html

[R35] 后台执行并等待
来源：http://hz.wangshuangyany.cn/gtkcmrttwt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.svipenyu.cn/gtfpddmkjn.html

[R36] 并发执行多个任务
来源：http://hz.shanyushiyangkeji.top/gtasezhron.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jqgfzy.top/gtpuxshzyv.html

[R37] 把输出赋给变量
来源：http://hz.quarkkingdee.top/gtcfohlyiw.html

files=$(ls -1)
来源：http://hz.yuanzhike.top/gtuzyhvuuq.html

[R38] 管道串联
来源：http://hz.pycfn.com/gtllfiqqet.html

cat a.txt | grep -i error | wc -l
来源：http://hz.nanxinkj.top/gtgurbrpbm.html

[R39] 重定向标准输出与错误
来源：http://hz.sweek.top/gteliwmdhi.html

cmd > out.log 2>&1
来源：http://hz.xingfuxueyuan.xyz/gtuwcdatim.html

[R40] 追加写日志
来源：http://hz.guowangkeji.top/gteiemkmcv.html

echo "log" >> out.log
来源：http://hz.yj202588.top/gtuxsvyari.html

[R41] 丢弃输出
来源：http://hz.havefunace.top/gtjfpdcmpm.html

cmd >/dev/null 2>&1
来源：http://hz.fengsongda.top/gtngdhrpxv.html

[R42] 输入重定向
来源：http://hz.shuidangran.top/gtoopnlbgq.html

wc -l < a.txt
来源：http://hz.tian-w.cn/gtmvghmljc.html

[R43] 按名字查找文件
来源：http://hz.shanyushiyangtech.top/gtgjmzuymt.html

find . -name "*.log" -type f
来源：http://hz.jinqigufen.top/gthdphywza.html

[R44] 按修改时间查找
来源：http://hz.jqgufenzy.top/gttixcewwa.html

find . -mtime -7 -type f
来源：http://hz.yueranfly.top/gtghxbecew.html

[R45] 批量删除
来源：http://hz.birdmap.top/gtrcxrzuou.html

find . -name "*.tmp" -delete
来源：http://hz.xuetiantiany.cn/gtwmniazxy.html

[R46] 递归替换文件内容
来源：http://hz.sufxvd.cn/gthzjizzao.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.havefunace.top/gtlcrnxthn.html

[R47] sed 单行替换
来源：http://hz.tanke756.top/gtvbfkiopn.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.chenlongwang.top/gtwfmjoohb.html

[R48] awk 取指定列
来源：http://hz.zdqjudy.top/gtxernisad.html

awk '{print $1, $3}' a.txt
来源：http://hz.shangyingyoupin.top/gtagsuavpu.html

[R49] awk 带条件
来源：http://hz.jlsjyb.cn/gtvbazgidw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.c1oappe.top/gtaqyjgyda.html

[R50] awk 求和
来源：http://hz.gogol.net.cn/gtoarlaapx.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.gogol.net.cn/gtgzpcqmpi.html

[R51] 排序去重取前几
来源：http://hz.mhx1999.top/gtnqwdexdf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.xingfuxueyuan.xyz/gtizikvvff.html

[R52] 统计行数
来源：http://hz.xziqi.cn/gtoxzjkrcj.html

wc -l a.txt
来源：http://hz.hfpthk.cn/gtqbjrnnkk.html

[R53] 查看文件头与实时尾
来源：http://hz.xuanzx.com/gtfxluybxr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.meibo888.top/gtcynkoyia.html

[R54] 比较两个文件
来源：http://hz.zhixingplan.top/gtrqvpofaq.html

diff a.txt b.txt
来源：http://hz.cashguo.top/gtfslxjdzm.html

[R55] 压缩与解压
来源：http://hz.chenzaomai.com/gtuutnpojf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.tanke756.top/gtatqhpwfo.html

[R56] 远程拷贝
来源：http://hz.shanyushiyangtech.top/gtupivtjck.html

scp file user@host:/path/
来源：http://hz.tianlin.xyz/gtwuspfiit.html

[R57] 远程执行命令
来源：http://hz.shangyingyoupin.top/gtrpzwnczb.html

ssh user@host 'uptime'
来源：http://hz.chenjidiqi.icu/gtmpztwtpo.html

[R58] 下载文件
来源：http://hz.zhengqikj.top/gtgzktvcug.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jinqigfzy.top/gtxtzcdlpx.html

[R59] 发 POST JSON
来源：http://hz.zhaomingkeji.xyz/gtlztaaxgm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shangyingyoupin.top/gtqfvxzupf.html

[R60] 只看 HTTP 状态码
来源：http://hz.chenlongwang.top/gtnkbmuxkv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.cdnleiting.top/gtkytbxwxi.html

[R61] 磁盘占用
来源：http://hz.aizwys.cn/gtmamxjqch.html

df -h;  du -sh *
来源：http://hz.zdqjudy.top/gtvhqtdiux.html

[R62] 找最占空间的文件
来源：http://hz.ehwqpu.com/gtdyqlndpb.html

du -ah . | sort -rh | head -10
来源：http://hz.ybcxt.top/gtyryzmcdd.html

[R63] 内存与进程
来源：http://hz.bjfxy.top/gtlpfzxlfe.html

free -h;  ps aux | grep nginx
来源：http://hz.hnqzz.top/gtajscxyvk.html

[R64] 结束进程
来源：http://hz.jyoumei.cn/gtzekwpuoy.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ppjwa.cn/gtbbhkawus.html

[R65] 查看端口占用
来源：http://hz.cqqwz.cn/gtfmnqcurv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ydzc1.top/gtsxgakrdi.html

[R66] 定时任务
来源：http://hz.jinghuilouyu.cn/gtynqnakih.html

crontab -e;  crontab -l
来源：http://hz.meibo888.top/gtehzfihks.html

[R67] 生成随机十六进制串
来源：http://hz.cdnleiting.top/gthwzmotnn.html

openssl rand -hex 16
来源：http://hz.dianchejie.cn/gthizliupm.html

[R68] 计算文件校验值
来源：http://hz.316326.xyz/gtvxkrpzvx.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shuidangran.top/gtmtmbeikz.html

[R69] 生成随机密码
来源：http://hz.wangdashe.top/gtrwlzotuc.html

head -c 16 /dev/urandom | base64
来源：http://hz.jinghuilouyu.cn/gtgjgsyyvf.html

[R70] 时间戳与互转
来源：http://hz.zhongyouzk.top/gtxhiqcwbq.html

date +%s;  date -d @1700000000
来源：http://hz.aibaodan.cn/gtdqgagxyl.html

[R71] 日期格式化
来源：http://hz.dashuyun.cn/gtcqbobxpr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zhijiandao.cn/gtktqriyoc.html

[R72] 等待端口就绪
来源：http://hz.sxryk.cn/gturzgqrxd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.vqdsnc.cn/gteyeweasi.html

[R73] 分割大日志
来源：http://hz.xziqi.cn/gtnmradfjw.html

split -l 1000 big.log part_
来源：http://hz.jqgfzy.top/gtnmpiaujb.html

[R74] 批量重命名
来源：http://hz.cucudq.cn/gthkncpxch.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.redwolf501.top/gtuyfljvxt.html

[R75] 导出环境变量
来源：http://hz.xingfuxueyuan.xyz/gtociilfgf.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.iojbl.cn/gttgeksqgp.html

[R76] 使用临时文件
来源：http://hz.shuidangran.top/gtckoafyzy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gogol.net.cn/gtmutavwos.html

[R77] 读取用户输入
来源：http://hz.yueranfly.top/gtnzisevvv.html

read -rp "请输入: " ans
来源：http://hz.xuetiantiany.cn/gticqmupiq.html

[R78] 交互式菜单
来源：http://hz.chenzaomai.com/gtwfotjolc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xziqi.cn/gtgnihxtkk.html

[R79] 解析命令行选项
来源：http://hz.sxryk.cn/gtrmscwecw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.pycfn.com/gtmewaflso.html

[R80] 查看脚本执行耗时
来源：http://hz.cheryme.top/gtxobufvmw.html

time ./run.sh
来源：http://hz.wangshuangyany.cn/gtmxvvehra.html

================================================================================
来源：http://hz.iojbl.cn/gtpgngvgsd.html

S. C / C++ 专题
来源：http://hz.ivvv.top/gtqarwodzq.html

================================================================================
来源：http://hz.havefunace.top/gtqkflrdjx.html

[S01] C：Hello World
来源：http://hz.hfpthk.cn/gtjjhrcdto.html

#include <stdio.h>
来源：http://hz.kuanghao11.cn/gtlflbhkdi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.snrcjt.cn/gtrtkwswee.html

[S02] C：变量与格式化输出
来源：http://hz.hywenlv.cn/gtsvwyrvrx.html

int a = 10; printf("%d\n", a);
来源：http://hz.smart0.xyz/gtdffdjvhg.html

[S03] C：读入整数
来源：http://hz.smart0.xyz/gtadrvnkvx.html

int x; scanf("%d", &x);
来源：http://hz.xingfuxueyuan.xyz/gtyvuclidh.html

[S04] C：字符串复制
来源：http://hz.ybcxt.top/gtmrwqzuxl.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zycfv.cn/gtdsztngwe.html

[S05] C：字符串长度
来源：http://hz.aibaodan.cn/gtdvrjyzvp.html

strlen(s)
来源：http://hz.jqgfzy.top/gtkhdpwxxv.html

[S06] C：字符串比较
来源：http://hz.ybcxt.top/gtegalywva.html

strcmp(a, b) == 0
来源：http://hz.guannengcc.top/gtpifdogxl.html

[S07] C：数组遍历求和
来源：http://hz.xinyue.icu/gtchrpffvp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jinqigufen.top/gtzhcayikx.html

[S08] C：动态内存分配与释放
来源：http://hz.snrcjt.cn/gtubyagato.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ydjk.org.cn/gtxjdxhtms.html

[S09] C：结构体定义与初始化
来源：http://hz.kuanghao11.cn/gtafzvolqr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.daxiang520.top/gtzhhxywka.html

[S10] C：指针与解引用
来源：http://hz.yongpay.top/gthstsdpoj.html

int *p = &a;  *p = 5;
来源：http://hz.shangyingyoupin.top/gtisqomvzt.html

[S11] C：逐行读文件
来源：http://hz.zdqjudy.top/gtvprrqeih.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jqgufenzy.top/gtxzdwnwjx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.0kj1m.cn/gtiqwupydi.html

fclose(f);
来源：http://hz.hammf.cn/gtisbqmyhu.html

[S12] C：写文件
来源：http://hz.snrcjt.cn/gtruzkdzbd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xinyue.icu/gthwnndwyy.html

[S13] C：宏定义
来源：http://hz.hfpthk.cn/gtnqtvyfvy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ydzc1.top/gtllnezkkc.html

[S14] C：枚举
来源：http://hz.shanyushiyangtech.top/gtqwgdxboe.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhijiandao.cn/gtrrmzkisn.html

[S15] C：类型转换
来源：http://hz.zhoulong.xyz/gtwdytdcmr.html

(double) a / b
来源：http://hz.pengpengdd.cyou/gtaufojsbq.html

[S16] C：位操作置位
来源：http://hz.ybcxt.top/gtovtgiqcj.html

x |= (1 << 3);
来源：http://hz.hywenlv.cn/gtrypjcmtm.html

[S17] C：安全拼接字符串
来源：http://hz.hnxiangtu.top/gtoizthtih.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.nanxinkj.top/gtfvbuwbog.html

[S18] C：命令行参数
来源：http://hz.yongpay.top/gtrysxwjno.html

int main(int argc, char **argv)
来源：http://hz.ybcxt.top/gtpyxdkjnc.html

[S19] C：快速排序
来源：http://hz.sysykeji.top/gtkoaamerb.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hongshengwenyu.top/gtlrowbrzo.html

[S20] C：二分查找
来源：http://hz.smart0.xyz/gtjscxsuyf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jqgufenzy.top/gtkseyaure.html

[S21] C：字符类别判断
来源：http://hz.nanxinkj.top/gtopfebaqm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yonumen.top/gtpohyzpqz.html

[S22] C：字符串转数字
来源：http://hz.fzhhl.top/gtefrxehjr.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yuxming.cn/gtizjqomwc.html

[S23] C：随机数
来源：http://hz.shanyushiyangkeji.top/gtxbgfqlzu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cqqwz.cn/gtaiaudqbw.html

[S24] C：获取本地时间
来源：http://hz.316326.xyz/gtcnswyvev.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.sufxvd.cn/gtwhwmulzh.html

[S25] C：内存拷贝
来源：http://hz.zycfv.cn/gttonpukle.html

memcpy(dst, src, n);
来源：http://hz.zhiwuduotai.top/gtonzxulvy.html

[S26] C：内存清零
来源：http://hz.ybcxt.top/gtdhxrwzad.html

memset(a, 0, sizeof a);
来源：http://hz.yonumen.top/gtuiprftnn.html

[S27] C：定义常量
来源：http://hz.quarkkingdee.top/gtsppdyedf.html

const double PI = 3.14159;
来源：http://hz.c1oappe.top/gtbngeaugo.html

[S28] C：静态变量
来源：http://hz.sweek.top/gtvidwxsed.html

static int counter = 0;
来源：http://hz.yueranfly.top/gtesqfncow.html

[S29] C：变参函数
来源：http://hz.gzhubu.top/gtucesmqic.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhixingplan.top/gtvhkyklgu.html

[S30] C：头文件保护
来源：http://hz.zhixingplan.top/gtceerbhdv.html

#ifndef X_H
来源：http://hz.chenzaomai.com/gtkorpmbdc.html

#define X_H
来源：http://hz.sysykeji.top/gtukxckstn.html

#endif
来源：http://hz.yongpay.top/gtmdycqorb.html

[S31] C++：Hello World
来源：http://hz.aibaodan.cn/gtpnyvxhvs.html

#include <iostream>
来源：http://hz.iojbl.cn/gtjbzugzrz.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jiagoushi.top/gtrufghjjx.html

[S32] C++：字符串
来源：http://hz.yuxming.cn/gtvxwgdzvw.html

std::string s = "hi";  s += "!";
来源：http://hz.vqdsnc.cn/gtqirwaedw.html

[S33] C++：vector 增删
来源：http://hz.hongshengwenyu.top/gtbujqkdqb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.52xcode.cn/gtcsgkbiae.html

[S34] C++：遍历 vector
来源：http://hz.guowangkeji.top/gtxmuvqcvs.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zycfv.cn/gtnwxmmgbn.html

[S35] C++：map
来源：http://hz.gotoacloud.top/gtxdxekgxl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ivvv.top/gtmngonela.html

[S36] C++：unordered_map
来源：http://hz.snrcjt.cn/gtaiefoojy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nanxinkj.top/gtkomlgbtq.html

[S37] C++：set
来源：http://hz.jiagoushi.top/gtpxsseqnf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yuxming.cn/gttfpousxh.html

[S38] C++：排序
来源：http://hz.yj202588.top/gtmihmpyjs.html

std::sort(v.begin(), v.end());
来源：http://hz.yj20258888.top/gtdohclsir.html

[S39] C++：自定义比较器排序
来源：http://hz.nanxuanxn.top/gtxsbnuppw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.sysykeji.top/gtekuiaqrq.html

[S40] C++：查找元素
来源：http://hz.aibaodan.cn/gtsxdsevra.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xylfe.cn/gthnpywjik.html

[S41] C++：类与构造函数
来源：http://hz.ppjwa.cn/gtcdwgjwjz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.aibaodan.cn/gtwtxpnlbv.html

[S42] C++：继承与虚函数
来源：http://hz.cashguo.top/gtngnffxzi.html

class B : public Base { public: void f() override {} };
来源：http://hz.fengsongda.top/gttkcmatzt.html

[S43] C++：智能指针
来源：http://hz.yanxiufei.cn/gttdifrhcz.html

auto p = std::make_unique<int>(5);
来源：http://hz.nanxinkj.top/gtfbjzbhxo.html

[S44] C++：引用传参
来源：http://hz.mhx1999.top/gtanbvcgte.html

void inc(int &x) { ++x; }
来源：http://hz.dianchejie.cn/gtwaiopdzw.html

[S45] C++：lambda
来源：http://hz.hnxiangtu.top/gtzyixkxpn.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.feifeiyinyue.top/gtxrhrslvh.html

[S46] C++：函数模板
来源：http://hz.vqdsnc.cn/gtfoqypjir.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.xuetiantiany.cn/gtnuuehcsf.html

[S47] C++：结构化绑定遍历
来源：http://hz.wangdashe.top/gtuuxhsfeq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.tian-w.cn/gtgprmrlzu.html

[S48] C++：逐行读文件
来源：http://hz.wangdashe.top/gtdfkvuuuc.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.316326.xyz/gtynqlrqyg.html

while (std::getline(in, line)) { }
来源：http://hz.jqgufenzy.top/gtyylvzuca.html

[S49] C++：写文件
来源：http://hz.zhiwuduotai.top/gtumgmlmfg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jyoumei.cn/gtssoggogz.html

[S50] C++：格式化数字
来源：http://hz.fengsongda.top/gtkzoztodg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.gaohongyu789.top/gtfddlqdrm.html

[S51] C++：显式类型转换
来源：http://hz.meibo888.top/gtbavvtlcm.html

static_cast<double>(a) / b
来源：http://hz.jyoumei.cn/gtkuxkwbar.html

[S52] C++：const 与 noexcept
来源：http://hz.snrcjt.cn/gtarevegzv.html

int size() const noexcept { return n_; }
来源：http://hz.ivvv.top/gtvtuotsrj.html

[S53] C++：移动语义
来源：http://hz.aizwys.cn/gteqdttsjr.html

std::vector<int> w = std::move(v);
来源：http://hz.zhoulong.xyz/gtdhkrelig.html

[S54] C++：异常处理
来源：http://hz.tian-w.cn/gtaefwywmk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.quarkkingdee.top/gtqurafhef.html

[S55] C++：结构化绑定
来源：http://hz.jqgufenzy.top/gtxysbvmpa.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhiwuduotai.top/gtzjgklhpl.html

[S56] C++：optional
来源：http://hz.316326.xyz/gtycbbjxry.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.0kj1m.cn/gtgltztddc.html

[S57] C++：编译期常量
来源：http://hz.zhaomingkeji.xyz/gtvsexafia.html

constexpr int N = 10;
来源：http://hz.cucudq.cn/gtlnacnwgv.html

[S58] C++：命名空间
来源：http://hz.xziqi.cn/gtxedbmrls.html


<!-- 参考信息 -->