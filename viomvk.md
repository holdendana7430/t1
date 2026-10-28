代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://hz.hnxiangtu.top/gtptdgxsjg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhoulong.xyz/gtizvqbbry.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.iojbl.cn/gtziiktakv.html

[Q89] 判断表是否存在
来源：http://hz.yonumen.top/gtdwjkehfe.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.shzxlz.cn/gtjexhlknh.html

[Q90] 生成序号列
来源：http://hz.xinyue.icu/gtknxaankz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.bjfxy.top/gtjiapjufo.html

================================================================================
来源：http://hz.quarkkingdee.top/gtkratgryi.html

R. Bash 专题
来源：http://hz.jiagoushi.top/gtrdxvuzpa.html

================================================================================
来源：http://hz.zdqjudy.top/gtdenongns.html

[R01] shebang 与严格模式
来源：http://hz.iojbl.cn/gtukzogbef.html

#!/usr/bin/env bash
来源：http://hz.fengsongda.top/gtxvhwmdvs.html

set -euo pipefail
来源：http://hz.pycfn.com/gtckxtlojc.html

[R02] 变量赋值与使用
来源：http://hz.yanxiufei.cn/gtxzbywgun.html

name="Tom"; echo "$name"
来源：http://hz.yuanzhike.top/gtihrjuufl.html

[R03] 只读变量
来源：http://hz.jinyuanbaomall.cn/gtzicmfsuq.html

readonly PI=3.14
来源：http://hz.xylfe.cn/gtosxzfseb.html

[R04] 位置参数
来源：http://hz.hnxiangtu.top/gtbuxpgart.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.svipenyu.cn/gttvtwwurn.html

[R05] 参数默认值
来源：http://hz.hfpthk.cn/gtiqhcfdpl.html

name="${1:-default}"
来源：http://hz.hywenlv.cn/gtgujbhlfo.html

[R06] 判断命令是否存在
来源：http://hz.aibaodan.cn/gtshdvcvvm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhengqikj.top/gtridmtvwb.html

[R07] if 判断文件
来源：http://hz.xuetiantiany.cn/gtvhwplpit.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.chenjidiqi.icu/gtpaxzvxzc.html

[R08] 数值比较
来源：http://hz.hysaishi.cn/gtrzzitvox.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.316326.xyz/gtkgralyvp.html

[R09] 字符串比较
来源：http://hz.zhoulong.xyz/gtapviwvdp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.shangyingyoupin.top/gtktzkvgrn.html

[R10] 正则匹配
来源：http://hz.zhaomingkeji.xyz/gtyizykpfs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.kuanghao11.cn/gtuqmpxupz.html

[R11] case 多分支
来源：http://hz.zdqjudy.top/gtyenahsxe.html

case "$1" in
来源：http://hz.cheryme.top/gtmzzjyjho.html

start) echo "启动" ;;
来源：http://hz.tian-w.cn/gtsctugzyr.html

stop)  echo "停止" ;;
来源：http://hz.daxiang520.top/gtpgjyagqn.html

*)     echo "未知命令" ;;
来源：http://hz.sysykeji.top/gtjnrveluk.html

esac
来源：http://hz.fengsongda.top/gtapllffyf.html

[R12] for 遍历文件
来源：http://hz.daria6918.cn/gtpmjajike.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yuanzhike.top/gtyergunco.html

[R13] for 计数循环
来源：http://hz.ywan-chungtsiang.top/gtvkjwwbys.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.kuanghao11.cn/gtuxxhwulk.html

[R14] C 风格 for
来源：http://hz.nanxuanxn.top/gtpziumnmk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yj20258888.top/gtpznijgjy.html

[R15] while 逐行读文件
来源：http://hz.smart0.xyz/gtorleklsf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jiagoushi.top/gtsznitehh.html

[R16] until 等待条件
来源：http://hz.yongpay.top/gtatpjhgjy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.sysykeji.top/gtpnwjaacq.html

[R17] 数组定义与取值
来源：http://hz.jinghuilouyu.cn/gteepqgnpt.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.tian-w.cn/gtwddpdahx.html

[R18] 遍历数组
来源：http://hz.tanke756.top/gtqbwiezix.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jinqigufen.top/gtfbtjillk.html

[R19] 数组长度
来源：http://hz.zhiwuduotai.top/gttustjjdo.html

echo "${#arr[@]}"
来源：http://hz.mhx1999.top/gtowpbjfep.html

[R20] 关联数组（字典）
来源：http://hz.wangshuangyany.cn/gtbenwwglr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.gogol.net.cn/gtebfexqfa.html

[R21] 字符串长度
来源：http://hz.kuanghao11.cn/gtdvbqnpdx.html

echo "${#s}"
来源：http://hz.birdmap.top/gtovowxrjs.html

[R22] 截取子串
来源：http://hz.zhengqikj.top/gtakslbjkm.html

echo "${s:0:5}"
来源：http://hz.chenlongwang.top/gtxltgqcnv.html

[R23] 字符串替换
来源：http://hz.52xcode.cn/gtfhvwhvts.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.cashguo.top/gtgcqgjkuo.html

[R24] 大小写转换
来源：http://hz.vqdsnc.cn/gtvettznxo.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.bjfxy.top/gtfazjgjvm.html

[R25] 去后缀 / 去前缀
来源：http://hz.pengpengdd.cyou/gtnbtamfwe.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.sufxvd.cn/gtvwcodzco.html

[R26] 命令替换
来源：http://hz.jianghu66.top/gtomhzoabd.html

now=$(date +%F); echo "$now"
来源：http://hz.xylfe.cn/gtikmvxsfo.html

[R27] 算术展开
来源：http://hz.xingfuxueyuan.xyz/gtvuykqjiq.html

echo $((1 + 2 * 3))
来源：http://hz.bjfxy.top/gtczehpeyk.html

[R28] 浮点运算
来源：http://hz.mhx1999.top/gtkodhnfhq.html

echo "scale=2; 10/3" | bc
来源：http://hz.nanxuanxn.top/gtbsgpcgcv.html

[R29] 定义函数
来源：http://hz.tanke756.top/gtjusybaxt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.mhx1999.top/gtxjanktqs.html

[R30] 函数返回状态码
来源：http://hz.hfpthk.cn/gtrbtxyshd.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ppjwa.cn/gteudechsh.html

[R31] 局部变量
来源：http://hz.bjfxy.top/gteapdtcxv.html

f() { local x=1; echo "$x"; }
来源：http://hz.jinqigfzy.top/gtdhxytqbj.html

[R32] 参数个数校验
来源：http://hz.gotoacloud.top/gtvwllhtjz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hammf.cn/gtqjpdzhsv.html

[R33] 捕获错误并提示行号
来源：http://hz.52xcode.cn/gtqipavufl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.hongshengwenyu.top/gthnecnzwi.html

[R34] 退出时清理
来源：http://hz.zhixingplan.top/gtkelcsssb.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.redwolf501.top/gtfoxrdauu.html

[R35] 后台执行并等待
来源：http://hz.ivvv.top/gtuusseeoe.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hammf.cn/gtiaadrtpn.html

[R36] 并发执行多个任务
来源：http://hz.havefunace.top/gtgrbhrlgz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jyoumei.cn/gtxfnsqyzh.html

[R37] 把输出赋给变量
来源：http://hz.birdmap.top/gtqlehgzxy.html

files=$(ls -1)
来源：http://hz.jinyuanbaomall.cn/gtrcmximvv.html

[R38] 管道串联
来源：http://hz.tian-w.cn/gtrmrlaxre.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhaomingkeji.xyz/gtksagybrj.html

[R39] 重定向标准输出与错误
来源：http://hz.ehwqpu.com/gtzrvucizs.html

cmd > out.log 2>&1
来源：http://hz.dashuyun.cn/gtmusxckpr.html

[R40] 追加写日志
来源：http://hz.gotoacloud.top/gtwqknxchq.html

echo "log" >> out.log
来源：http://hz.cheryme.top/gtvgocxbet.html

[R41] 丢弃输出
来源：http://hz.ydzc1.top/gtzhqvercf.html

cmd >/dev/null 2>&1
来源：http://hz.52xcode.cn/gthtaslhnx.html

[R42] 输入重定向
来源：http://hz.shuidangran.top/gtdnuvijwf.html

wc -l < a.txt
来源：http://hz.bjfxy.top/gtjtbzkeku.html

[R43] 按名字查找文件
来源：http://hz.zycfv.cn/gtndokyfos.html

find . -name "*.log" -type f
来源：http://hz.aizwys.cn/gtikqlpdju.html

[R44] 按修改时间查找
来源：http://hz.meibo888.top/gttyzqcwif.html

find . -mtime -7 -type f
来源：http://hz.yongpay.top/gtpkiucazc.html

[R45] 批量删除
来源：http://hz.daria6918.cn/gtjxwoznkf.html

find . -name "*.tmp" -delete
来源：http://hz.chenzaomai.com/gtkxtqhwwn.html

[R46] 递归替换文件内容
来源：http://hz.haohaochexian.top/gtwdfajqca.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.tian-w.cn/gtqpsuqbxl.html

[R47] sed 单行替换
来源：http://hz.ywan-chungtsiang.top/gtzuzhkwsg.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.nwbrower.top/gtyouivjyh.html

[R48] awk 取指定列
来源：http://hz.zhoulong.xyz/gthgoiocdx.html

awk '{print $1, $3}' a.txt
来源：http://hz.smart0.xyz/gtgkbgnlek.html

[R49] awk 带条件
来源：http://hz.yongpay.top/gtiregpyqj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ydjk.org.cn/gtehjzvrzg.html

[R50] awk 求和
来源：http://hz.bjfxy.top/gtrhloxxfh.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.wangdashe.top/gthubtwoud.html

[R51] 排序去重取前几
来源：http://hz.yj20258.top/gtibqceado.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zycfv.cn/gtdzdxjdsp.html

[R52] 统计行数
来源：http://hz.chenzaomai.com/gtvwmjeymj.html

wc -l a.txt
来源：http://hz.9152youxi.cn/gtvgxzmuel.html

[R53] 查看文件头与实时尾
来源：http://hz.mhx1999.top/gtjuxtjcbo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.birdmap.top/gttmbtbzwu.html

[R54] 比较两个文件
来源：http://hz.hammf.cn/gtdaknwplw.html

diff a.txt b.txt
来源：http://hz.quarkkingdee.top/gtbucmxrnj.html

[R55] 压缩与解压
来源：http://hz.zhoulong.xyz/gtzqfanfkm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.nanxuanxn.top/gtfxqcslcb.html

[R56] 远程拷贝
来源：http://hz.ydzc1.top/gtvoulhsdx.html

scp file user@host:/path/
来源：http://hz.jiagoushi.top/gtqxannwoe.html

[R57] 远程执行命令
来源：http://hz.iojbl.cn/gtfjbrmpye.html

ssh user@host 'uptime'
来源：http://hz.yongpay.top/gtwttfmwyd.html

[R58] 下载文件
来源：http://hz.shangyingyoupin.top/gtiztkckhk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.quarkkingdee.top/gtpbtcoysg.html

[R59] 发 POST JSON
来源：http://hz.jinghuilouyu.cn/gtoimqkmrq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.0kj1m.cn/gtgbpjqrat.html

[R60] 只看 HTTP 状态码
来源：http://hz.gogol.net.cn/gtdctmmuas.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.pycfn.com/gtgzqtenbx.html

[R61] 磁盘占用
来源：http://hz.vqdsnc.cn/gtvpdpexpr.html

df -h;  du -sh *
来源：http://hz.nanxinkj.top/gthmixwuhs.html

[R62] 找最占空间的文件
来源：http://hz.hongshengwenyu.top/gtqfgcbkqr.html

du -ah . | sort -rh | head -10
来源：http://hz.zhijiandao.cn/gtysutpvkq.html

[R63] 内存与进程
来源：http://hz.ywan-chungtsiang.top/gtrgezjdvq.html

free -h;  ps aux | grep nginx
来源：http://hz.ydzc1.top/gtapvplndh.html

[R64] 结束进程
来源：http://hz.quarkkingdee.top/gtkxrngkar.html

kill -9 $(pgrep -f app.py)
来源：http://hz.guowangkeji.top/gtnxzuoejv.html

[R65] 查看端口占用
来源：http://hz.yonumen.top/gtejexlmjs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.kuanghao11.cn/gtgkiigfef.html

[R66] 定时任务
来源：http://hz.zhaomingkeji.xyz/gtnqsinlhu.html

crontab -e;  crontab -l
来源：http://hz.iojbl.cn/gtwufgfhdc.html

[R67] 生成随机十六进制串
来源：http://hz.daria6918.cn/gtfhmlhxbm.html

openssl rand -hex 16
来源：http://hz.cqqwz.cn/gtwilrmpoa.html

[R68] 计算文件校验值
来源：http://hz.zhixingplan.top/gtxxiyjzvf.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.iojbl.cn/gtspruiwww.html

[R69] 生成随机密码
来源：http://hz.feifeiyinyue.top/gttqmgyjzt.html

head -c 16 /dev/urandom | base64
来源：http://hz.quarkkingdee.top/gtarinojpi.html

[R70] 时间戳与互转
来源：http://hz.cashguo.top/gthrxumswq.html

date +%s;  date -d @1700000000
来源：http://hz.tianlin.xyz/gtxblvicnw.html

[R71] 日期格式化
来源：http://hz.jinqigfzy.top/gtvkxgndnv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.wangshuangyany.cn/gtttjxwltv.html

[R72] 等待端口就绪
来源：http://hz.yangfankeji.com/gtnzncwjql.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jinqigfzy.top/gtomoaalsq.html

[R73] 分割大日志
来源：http://hz.mhx1999.top/gtdwbepwzz.html

split -l 1000 big.log part_
来源：http://hz.yj20258.top/gtwgznsirf.html

[R74] 批量重命名
来源：http://hz.redwolf501.top/gtgyoabtpi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.snrcjt.cn/gtdvbkqdct.html

[R75] 导出环境变量
来源：http://hz.yj20258888.top/gtgttrmpim.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zycfv.cn/gtrpdyonms.html

[R76] 使用临时文件
来源：http://hz.yuanzhike.top/gtuynerntn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinghuilouyu.cn/gtzrfcaqcn.html

[R77] 读取用户输入
来源：http://hz.gotoacloud.top/gtwjugsdkg.html

read -rp "请输入: " ans
来源：http://hz.ybcxt.top/gtonvrusdt.html

[R78] 交互式菜单
来源：http://hz.chenzaomai.com/gthrmuwgkg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hywenlv.cn/gtfbtewhex.html

[R79] 解析命令行选项
来源：http://hz.vqdsnc.cn/gthbiyhiwj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.smart0.xyz/gtdbamfult.html

[R80] 查看脚本执行耗时
来源：http://hz.chenzaomai.com/gtjjqdwpme.html

time ./run.sh
来源：http://hz.jiagoushi.top/gtjtgdapow.html

================================================================================
来源：http://hz.hfpthk.cn/gtlrtjrgit.html

S. C / C++ 专题
来源：http://hz.havefunace.top/gtuveyxexp.html

================================================================================
来源：http://hz.gogol.net.cn/gtfwroigjo.html

[S01] C：Hello World
来源：http://hz.xuetiantiany.cn/gtzskjxilx.html

#include <stdio.h>
来源：http://hz.pengpengdd.cyou/gtzugjfwfm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.dashuyun.cn/gtpdjfnjtz.html

[S02] C：变量与格式化输出
来源：http://hz.tian-w.cn/gtevfoureg.html

int a = 10; printf("%d\n", a);
来源：http://hz.xuetiantiany.cn/gtgbmhiohf.html

[S03] C：读入整数
来源：http://hz.shanyushiyangkeji.top/gtfilikwwp.html

int x; scanf("%d", &x);
来源：http://hz.shuidangran.top/gteltwrojl.html

[S04] C：字符串复制
来源：http://hz.gogol.net.cn/gtisrwofnx.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.daria6918.cn/gtrcbmpdra.html

[S05] C：字符串长度
来源：http://hz.redwolf501.top/gtpwmqbzfp.html

strlen(s)
来源：http://hz.feifeiyinyue.top/gttqrjxcfv.html

[S06] C：字符串比较
来源：http://hz.andypj.xyz/gtjwosxcsg.html

strcmp(a, b) == 0
来源：http://hz.wangshuangyany.cn/gtlwcstkyx.html

[S07] C：数组遍历求和
来源：http://hz.shanyushiyangkeji.top/gtfuhhnkwx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jqgfzy.top/gtsqvkopow.html

[S08] C：动态内存分配与释放
来源：http://hz.zhijiandao.cn/gteqbwklcm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.mhx1999.top/gtqslmqfey.html

[S09] C：结构体定义与初始化
来源：http://hz.hongshengwenyu.top/gtpuzdhkee.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ehwqpu.com/gtpvvgfoux.html

[S10] C：指针与解引用
来源：http://hz.dashuyun.cn/gtkhkdoluh.html

int *p = &a;  *p = 5;
来源：http://hz.hfpthk.cn/gtdkzqxgdy.html

[S11] C：逐行读文件
来源：http://hz.wangshuangyany.cn/gttyivpndg.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.pycfn.com/gtbmnprsab.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yuanzhike.top/gtouhikbbd.html

fclose(f);
来源：http://hz.svipenyu.cn/gtrtgdjhgl.html

[S12] C：写文件
来源：http://hz.zhijiandao.cn/gtnqeennks.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.shangyingyoupin.top/gtdpsxqxfl.html

[S13] C：宏定义
来源：http://hz.cashguo.top/gtmxxlybpc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.cucudq.cn/gthluobncc.html

[S14] C：枚举
来源：http://hz.sufxvd.cn/gtsrbszdcm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jyoumei.cn/gtzctnpgcv.html

[S15] C：类型转换
来源：http://hz.jyoumei.cn/gthfsearwo.html

(double) a / b
来源：http://hz.jqgufenzy.top/gtwfagizda.html

[S16] C：位操作置位
来源：http://hz.xylfe.cn/gtxhhwcndh.html

x |= (1 << 3);
来源：http://hz.tanke756.top/gtmmuhurfv.html

[S17] C：安全拼接字符串
来源：http://hz.52xcode.cn/gtboepqihn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.wangdashe.top/gtgpsueqdm.html

[S18] C：命令行参数
来源：http://hz.daria6918.cn/gtaqwyknmf.html

int main(int argc, char **argv)
来源：http://hz.jianghu66.top/gtbxspenpq.html

[S19] C：快速排序
来源：http://hz.9152youxi.cn/gtqvbmfwgz.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jlsjyb.cn/gtwluxovrk.html

[S20] C：二分查找
来源：http://hz.ehwqpu.com/gtqhlaxeiq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.52xcode.cn/gtlxtyjtoq.html

[S21] C：字符类别判断
来源：http://hz.hywenlv.cn/gtspooribz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jinqigfzy.top/gtufdyykra.html

[S22] C：字符串转数字
来源：http://hz.jianghu66.top/gtxljawtye.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.nanxuanxn.top/gtjatrhqml.html

[S23] C：随机数
来源：http://hz.shanyushiyangkeji.top/gtmbpaurfg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhaomingkeji.xyz/gtimqcbuab.html

[S24] C：获取本地时间
来源：http://hz.yuanzhike.top/gtwgmcxfjh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yonumen.top/gthhsgjhyl.html

[S25] C：内存拷贝
来源：http://hz.gaohongyu789.top/gtiinhygvq.html

memcpy(dst, src, n);
来源：http://hz.zycfv.cn/gtplifpavz.html

[S26] C：内存清零
来源：http://hz.zhijiandao.cn/gtjrsiqizk.html

memset(a, 0, sizeof a);
来源：http://hz.sweek.top/gtrndztezh.html

[S27] C：定义常量
来源：http://hz.yonumen.top/gtzwstffsm.html

const double PI = 3.14159;
来源：http://hz.guannengcc.top/gtbfnwpdhz.html

[S28] C：静态变量
来源：http://hz.jqgfzy.top/gtbgbayrdq.html

static int counter = 0;
来源：http://hz.shanyushiyangtech.top/gtkvdwiggn.html

[S29] C：变参函数
来源：http://hz.yangfankeji.com/gtfivhvcco.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.pengpengdd.cyou/gtaatywqhx.html

[S30] C：头文件保护
来源：http://hz.zhiwuduotai.top/gtggepaqno.html

#ifndef X_H
来源：http://hz.guowangkeji.top/gtalkinymt.html

#define X_H
来源：http://hz.hfpthk.cn/gtilysdulw.html

#endif
来源：http://hz.feifeiyinyue.top/gtpcivfzix.html

[S31] C++：Hello World
来源：http://hz.zycfv.cn/gtvzinylpx.html

#include <iostream>
来源：http://hz.nwbrower.top/gtigatobio.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.shanyushiyangkeji.top/gtvuouxacm.html

[S32] C++：字符串
来源：http://hz.xuanzx.com/gtzxywzlrk.html

std::string s = "hi";  s += "!";
来源：http://hz.daxiang520.top/gtnwethpvn.html

[S33] C++：vector 增删
来源：http://hz.birdmap.top/gtknjosvtw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.tanke756.top/gtnrshkrbi.html

[S34] C++：遍历 vector
来源：http://hz.daxiang520.top/gtlydnpdqc.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jiagoushi.top/gtbhvafrfe.html

[S35] C++：map
来源：http://hz.fengsongda.top/gtqhwzcttv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhiwuduotai.top/gtwkwjwihp.html

[S36] C++：unordered_map
来源：http://hz.zhaomingkeji.xyz/gtwxsojmpo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhixingplan.top/gtcbuimvju.html

[S37] C++：set
来源：http://hz.smart0.xyz/gtulnreqig.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hywenlv.cn/gtzhkmmits.html

[S38] C++：排序
来源：http://hz.c1oappe.top/gtjjtjatmo.html

std::sort(v.begin(), v.end());
来源：http://hz.nanxinkj.top/gtylgukpgw.html

[S39] C++：自定义比较器排序
来源：http://hz.ybcxt.top/gtlvpnousp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.nwbrower.top/gtliawafcd.html

[S40] C++：查找元素
来源：http://hz.chenzaomai.com/gtiniiccaw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.gogol.net.cn/gtnkjhjnch.html

[S41] C++：类与构造函数
来源：http://hz.snrcjt.cn/gtrzgldtlr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yj202588.top/gtbdobwyum.html

[S42] C++：继承与虚函数
来源：http://hz.sweek.top/gtxcquyxuo.html

class B : public Base { public: void f() override {} };
来源：http://hz.ybcxt.top/gtykrnxqho.html

[S43] C++：智能指针
来源：http://hz.yanxiufei.cn/gtxxwjmzra.html

auto p = std::make_unique<int>(5);
来源：http://hz.gotoacloud.top/gtixjoozfc.html

[S44] C++：引用传参
来源：http://hz.jiagoushi.top/gtmxydpfgc.html

void inc(int &x) { ++x; }
来源：http://hz.cdnleiting.top/gtlmkkvslc.html

[S45] C++：lambda
来源：http://hz.zhengqikj.top/gtbdbexewc.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yvedp.cn/gtsptksrhm.html

[S46] C++：函数模板
来源：http://hz.pengpengdd.cyou/gtiwoongvb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ehwqpu.com/gtbsochfku.html

[S47] C++：结构化绑定遍历
来源：http://hz.tianlin.xyz/gtoipdileu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.fengsongda.top/gtqditiftz.html

[S48] C++：逐行读文件
来源：http://hz.jyoumei.cn/gtfrmjvras.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.chenjidiqi.icu/gtaslytwry.html

while (std::getline(in, line)) { }
来源：http://hz.vqdsnc.cn/gtecpyexxe.html

[S49] C++：写文件
来源：http://hz.zhixingplan.top/gtfjnezrxq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.pengpengdd.cyou/gtticnvccu.html

[S50] C++：格式化数字
来源：http://hz.zycfv.cn/gtjztehznv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.c1oappe.top/gtrbyzptpe.html

[S51] C++：显式类型转换
来源：http://hz.ybcxt.top/gtfwxnxgaq.html

static_cast<double>(a) / b
来源：http://hz.hnxiangtu.top/gtfzcqvstt.html

[S52] C++：const 与 noexcept
来源：http://hz.sweek.top/gtpjkbqxri.html

int size() const noexcept { return n_; }
来源：http://hz.ydzc1.top/gtsrqkzysb.html

[S53] C++：移动语义
来源：http://hz.aibaodan.cn/gtxajryqvn.html

std::vector<int> w = std::move(v);
来源：http://hz.bjfxy.top/gtybqqxkrr.html

[S54] C++：异常处理
来源：http://hz.hywenlv.cn/gtjyehfgon.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yanxiufei.cn/gtmdmcysvo.html

[S55] C++：结构化绑定
来源：http://hz.birdmap.top/gtrarsqlnu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.daxiang520.top/gtydhwvxkr.html

[S56] C++：optional
来源：http://hz.9152youxi.cn/gtlyuiaauj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.tian-w.cn/gtynenfegr.html

[S57] C++：编译期常量
来源：http://hz.shuidangran.top/gtlhdxktym.html

constexpr int N = 10;
来源：http://hz.fengsongda.top/gtbuwthshb.html

[S58] C++：命名空间
来源：http://hz.jlsjyb.cn/gtbjhxapam.html


<!-- 参考信息 -->