代发 wailian999

[Q86] 读取 JSON 字段
来源：http://hz.gzhubu.top/gtofqkzfno.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hywenlv.cn/gtssatduio.html

[Q87] JSON 字段做条件
来源：http://hz.ydjk.org.cn/gtrmgthnkq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ehwqpu.com/gtwpmrejyh.html

[Q88] 行转列（条件聚合）
来源：http://hz.guannengcc.top/gtmwebooxf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yangfankeji.com/gtkngrcxyo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jlsjyb.cn/gtrvehdruj.html

[Q89] 判断表是否存在
来源：http://hz.aibaodan.cn/gtfxifwcov.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.cheryme.top/gtqzldtkvq.html

[Q90] 生成序号列
来源：http://hz.xinyue.icu/gtoklsmjum.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.daria6918.cn/gttnzhzjxu.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtktgyzmgf.html

R. Bash 专题
来源：http://hz.shanyushiyangkeji.top/gtywurpklw.html

================================================================================
来源：http://hz.yj202588.top/gtmvynbrsq.html

[R01] shebang 与严格模式
来源：http://hz.cucudq.cn/gtxuxyaron.html

#!/usr/bin/env bash
来源：http://hz.birdmap.top/gtkexdefgh.html

set -euo pipefail
来源：http://hz.daxiang520.top/gtvoixedav.html

[R02] 变量赋值与使用
来源：http://hz.shuidangran.top/gtkmvrfxhn.html

name="Tom"; echo "$name"
来源：http://hz.meibo888.top/gtxauziida.html

[R03] 只读变量
来源：http://hz.xylfe.cn/gtbdfijugf.html

readonly PI=3.14
来源：http://hz.yangfankeji.com/gtmylbemcz.html

[R04] 位置参数
来源：http://hz.iojbl.cn/gthodfbbpd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.sysykeji.top/gtdruvjoqt.html

[R05] 参数默认值
来源：http://hz.ppjwa.cn/gtsluljjvq.html

name="${1:-default}"
来源：http://hz.hfpthk.cn/gtrdhqzpat.html

[R06] 判断命令是否存在
来源：http://hz.shzxlz.cn/gtbendimlh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.pycfn.com/gtaqgwupfj.html

[R07] if 判断文件
来源：http://hz.zhengqikj.top/gtlhvtofup.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hnxiangtu.top/gtxixfuokx.html

[R08] 数值比较
来源：http://hz.fengsongda.top/gtqxlkfudp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.feifeiyinyue.top/gtlsxyctqt.html

[R09] 字符串比较
来源：http://hz.jinyuanbaomall.cn/gteplgiwzb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.fzhhl.top/gtorssbefi.html

[R10] 正则匹配
来源：http://hz.nwbrower.top/gtkdodmszv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhaomingkeji.xyz/gtpwzvndzk.html

[R11] case 多分支
来源：http://hz.9152youxi.cn/gtldgayjpk.html

case "$1" in
来源：http://hz.zhijiandao.cn/gtecuwfyql.html

start) echo "启动" ;;
来源：http://hz.ydjk.org.cn/gtihsezwhw.html

stop)  echo "停止" ;;
来源：http://hz.jqgfzy.top/gtmytwdydg.html

*)     echo "未知命令" ;;
来源：http://hz.sxryk.cn/gtskcwvnys.html

esac
来源：http://hz.chenzaomai.com/gtokmzhbbu.html

[R12] for 遍历文件
来源：http://hz.pengpengdd.cyou/gtnaacjjtv.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yj20258888.top/gtvaehjrnn.html

[R13] for 计数循环
来源：http://hz.hongshengwenyu.top/gtxcxualoh.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.gzhubu.top/gtqxupovem.html

[R14] C 风格 for
来源：http://hz.redwolf501.top/gteavagebp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.0kj1m.cn/gttmxjxsdp.html

[R15] while 逐行读文件
来源：http://hz.vqdsnc.cn/gteueqnlzs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.cucudq.cn/gtmtqwzsws.html

[R16] until 等待条件
来源：http://hz.sufxvd.cn/gtvtixdqke.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ydzc1.top/gttvnaclgb.html

[R17] 数组定义与取值
来源：http://hz.xziqi.cn/gtbohdpxxl.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cdnleiting.top/gtbhpdqjgt.html

[R18] 遍历数组
来源：http://hz.dashuyun.cn/gtufteyvbo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jianghu66.top/gtwgigkxto.html

[R19] 数组长度
来源：http://hz.ydjk.org.cn/gtcvqomxum.html

echo "${#arr[@]}"
来源：http://hz.chenjidiqi.icu/gtynjvmkec.html

[R20] 关联数组（字典）
来源：http://hz.hfpthk.cn/gtvkhqxeil.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zycfv.cn/gtuwzayimt.html

[R21] 字符串长度
来源：http://hz.jqgufenzy.top/gtjrqhtagu.html

echo "${#s}"
来源：http://hz.jqgfzy.top/gthazpwsjy.html

[R22] 截取子串
来源：http://hz.smart0.xyz/gtcvojgkcf.html

echo "${s:0:5}"
来源：http://hz.jianghu66.top/gtyvcrjvds.html

[R23] 字符串替换
来源：http://hz.guowangkeji.top/gtgatkmfwj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.sufxvd.cn/gtswegwrpq.html

[R24] 大小写转换
来源：http://hz.yueranfly.top/gtzggspmcb.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.cqqwz.cn/gtnjcxloeq.html

[R25] 去后缀 / 去前缀
来源：http://hz.kuanghao11.cn/gtbjkwudhy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yueranfly.top/gtuvdmrfgn.html

[R26] 命令替换
来源：http://hz.hywenlv.cn/gtifqyjorj.html

now=$(date +%F); echo "$now"
来源：http://hz.hysaishi.cn/gtrizylbvf.html

[R27] 算术展开
来源：http://hz.guannengcc.top/gtidgflxbu.html

echo $((1 + 2 * 3))
来源：http://hz.cdnleiting.top/gtfnjfztec.html

[R28] 浮点运算
来源：http://hz.shanyushiyangkeji.top/gtcnjmvdvv.html

echo "scale=2; 10/3" | bc
来源：http://hz.316326.xyz/gtypjlaequ.html

[R29] 定义函数
来源：http://hz.mhx1999.top/gtdczpgmvk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xingfuxueyuan.xyz/gtyuxtdqlt.html

[R30] 函数返回状态码
来源：http://hz.xylfe.cn/gtriamemnp.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ydzc1.top/gtfapdhewa.html

[R31] 局部变量
来源：http://hz.aizwys.cn/gtrixavzyl.html

f() { local x=1; echo "$x"; }
来源：http://hz.hysaishi.cn/gteqmbgzdn.html

[R32] 参数个数校验
来源：http://hz.zhongyouzk.top/gtcktzalmo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.chenjidiqi.icu/gtkvgvbthm.html

[R33] 捕获错误并提示行号
来源：http://hz.bjfxy.top/gtneuhmekx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xingfuxueyuan.xyz/gtkljerwfw.html

[R34] 退出时清理
来源：http://hz.redwolf501.top/gtwjdewbrm.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.havefunace.top/gtgubgpemi.html

[R35] 后台执行并等待
来源：http://hz.gotoacloud.top/gtldmofgpc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xingfuxueyuan.xyz/gtvsytagyl.html

[R36] 并发执行多个任务
来源：http://hz.jinghuilouyu.cn/gthqlxeepd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jyoumei.cn/gtktsbizwn.html

[R37] 把输出赋给变量
来源：http://hz.wangshuangyany.cn/gtkmdkgqqn.html

files=$(ls -1)
来源：http://hz.kuanghao11.cn/gtywmimzjo.html

[R38] 管道串联
来源：http://hz.haohaochexian.top/gtratdjqxv.html

cat a.txt | grep -i error | wc -l
来源：http://hz.andypj.xyz/gtmkkawfiq.html

[R39] 重定向标准输出与错误
来源：http://hz.ywan-chungtsiang.top/gtouvbizfs.html

cmd > out.log 2>&1
来源：http://hz.feifeiyinyue.top/gteuoajpip.html

[R40] 追加写日志
来源：http://hz.jqgufenzy.top/gtlqujbfba.html

echo "log" >> out.log
来源：http://hz.jyoumei.cn/gtrqaoxjwe.html

[R41] 丢弃输出
来源：http://hz.jiagoushi.top/gtnpoeckmk.html

cmd >/dev/null 2>&1
来源：http://hz.chenjidiqi.icu/gthxdvuwec.html

[R42] 输入重定向
来源：http://hz.gogol.net.cn/gtdmhpypcp.html

wc -l < a.txt
来源：http://hz.jqgufenzy.top/gtkbzhjpvm.html

[R43] 按名字查找文件
来源：http://hz.sufxvd.cn/gtxuwbxncf.html

find . -name "*.log" -type f
来源：http://hz.meibo888.top/gtitsgmlnx.html

[R44] 按修改时间查找
来源：http://hz.dashuyun.cn/gttxenuygt.html

find . -mtime -7 -type f
来源：http://hz.tian-w.cn/gttrlqqaqs.html

[R45] 批量删除
来源：http://hz.daria6918.cn/gttavhxcmw.html

find . -name "*.tmp" -delete
来源：http://hz.yueranfly.top/gtlrnegrdw.html

[R46] 递归替换文件内容
来源：http://hz.hongshengwenyu.top/gtawzzkgog.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cheryme.top/gtenfglcus.html

[R47] sed 单行替换
来源：http://hz.jiagoushi.top/gtfmwdiixy.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jinyuanbaomall.cn/gtctyazrhf.html

[R48] awk 取指定列
来源：http://hz.vqdsnc.cn/gtjgkslxfy.html

awk '{print $1, $3}' a.txt
来源：http://hz.yonumen.top/gtzuuvhslb.html

[R49] awk 带条件
来源：http://hz.zhoulong.xyz/gtodmwzxpl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.shzxlz.cn/gttyelupks.html

[R50] awk 求和
来源：http://hz.52xcode.cn/gtecbodsiw.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.iojbl.cn/gtklbderca.html

[R51] 排序去重取前几
来源：http://hz.ydzc1.top/gtkrlvwwat.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yj20258.top/gtuxuivvvc.html

[R52] 统计行数
来源：http://hz.52xcode.cn/gtjezsuzno.html

wc -l a.txt
来源：http://hz.nanxinkj.top/gtbzphfggu.html

[R53] 查看文件头与实时尾
来源：http://hz.bjfxy.top/gtpezgcdcm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cashguo.top/gtgxxhykxq.html

[R54] 比较两个文件
来源：http://hz.gaohongyu789.top/gtfixjiwfb.html

diff a.txt b.txt
来源：http://hz.zhixingplan.top/gthwpknrtv.html

[R55] 压缩与解压
来源：http://hz.hysaishi.cn/gtrirbyurt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.daria6918.cn/gtonqhlcft.html

[R56] 远程拷贝
来源：http://hz.dashuyun.cn/gtuvzjdxht.html

scp file user@host:/path/
来源：http://hz.quarkkingdee.top/gtrlcjmubf.html

[R57] 远程执行命令
来源：http://hz.jinghuilouyu.cn/gtropfprpu.html

ssh user@host 'uptime'
来源：http://hz.yj20258888.top/gtbpewxejl.html

[R58] 下载文件
来源：http://hz.yanxiufei.cn/gtxxyjxdnl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.daria6918.cn/gtwlwzagnj.html

[R59] 发 POST JSON
来源：http://hz.tianlin.xyz/gtjpzmomcx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hywenlv.cn/gtoagfzged.html

[R60] 只看 HTTP 状态码
来源：http://hz.mhx1999.top/gtevremfmj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yongpay.top/gtogmdbnre.html

[R61] 磁盘占用
来源：http://hz.mhx1999.top/gtsevuonst.html

df -h;  du -sh *
来源：http://hz.zhengqikj.top/gtndleysjc.html

[R62] 找最占空间的文件
来源：http://hz.ydjk.org.cn/gtfsgwezhj.html

du -ah . | sort -rh | head -10
来源：http://hz.hnqzz.top/gtcpclmyis.html

[R63] 内存与进程
来源：http://hz.chenzaomai.com/gtbvzggpcu.html

free -h;  ps aux | grep nginx
来源：http://hz.shanyushiyangtech.top/gtkzlqrgwr.html

[R64] 结束进程
来源：http://hz.mhx1999.top/gtrnzkztih.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yueranfly.top/gtcmvrgpbf.html

[R65] 查看端口占用
来源：http://hz.pycfn.com/gtnmwyowfu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jiagoushi.top/gtpmfsngje.html

[R66] 定时任务
来源：http://hz.zhixingplan.top/gtjvzgvscy.html

crontab -e;  crontab -l
来源：http://hz.dianchejie.cn/gtopteaswc.html

[R67] 生成随机十六进制串
来源：http://hz.hfpthk.cn/gtmwqpmzde.html

openssl rand -hex 16
来源：http://hz.xziqi.cn/gtvrsqnzpf.html

[R68] 计算文件校验值
来源：http://hz.chenjidiqi.icu/gtmsnvkkuj.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.dianchejie.cn/gtnyexqaea.html

[R69] 生成随机密码
来源：http://hz.yj20258.top/gtwfeivshd.html

head -c 16 /dev/urandom | base64
来源：http://hz.xingfuxueyuan.xyz/gtnnjzulii.html

[R70] 时间戳与互转
来源：http://hz.shzxlz.cn/gtvrywhnmr.html

date +%s;  date -d @1700000000
来源：http://hz.cdnleiting.top/gtvlokuhzy.html

[R71] 日期格式化
来源：http://hz.yongpay.top/gthanwsjel.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.chenzaomai.com/gtbabhgqbh.html

[R72] 等待端口就绪
来源：http://hz.nanxuanxn.top/gtxkeersdj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.tian-w.cn/gtcxsxxrwq.html

[R73] 分割大日志
来源：http://hz.shangyingyoupin.top/gtftlkcsut.html

split -l 1000 big.log part_
来源：http://hz.yanxiufei.cn/gttwefcovf.html

[R74] 批量重命名
来源：http://hz.jianghu66.top/gtomxsejnk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jinqigfzy.top/gtnryulfei.html

[R75] 导出环境变量
来源：http://hz.svipenyu.cn/gtnccrmqxi.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yvedp.cn/gtuvlmfegr.html

[R76] 使用临时文件
来源：http://hz.xuetiantiany.cn/gtbkwvrefg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yvedp.cn/gtkqvizcxg.html

[R77] 读取用户输入
来源：http://hz.fzhhl.top/gtldjrjzrg.html

read -rp "请输入: " ans
来源：http://hz.bjfxy.top/gtftglpoxp.html

[R78] 交互式菜单
来源：http://hz.9152youxi.cn/gtivtkehzn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.chenlongwang.top/gtlfsjovwd.html

[R79] 解析命令行选项
来源：http://hz.hnqzz.top/gtmcejjddo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zhijiandao.cn/gtqwjxyudp.html

[R80] 查看脚本执行耗时
来源：http://hz.kuanghao11.cn/gtqakaizzx.html

time ./run.sh
来源：http://hz.gzhubu.top/gtfmiizmkk.html

================================================================================
来源：http://hz.yj202588.top/gtdzvwlopj.html

S. C / C++ 专题
来源：http://hz.shanyushiyangtech.top/gtrraifgcr.html

================================================================================
来源：http://hz.tian-w.cn/gttzzqabzd.html

[S01] C：Hello World
来源：http://hz.jianghu66.top/gtkqlzjhyb.html

#include <stdio.h>
来源：http://hz.jlsjyb.cn/gthwfcahai.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.fzhhl.top/gtwhpbacpd.html

[S02] C：变量与格式化输出
来源：http://hz.jinghuilouyu.cn/gtbsdwnxuu.html

int a = 10; printf("%d\n", a);
来源：http://hz.smart0.xyz/gtuupvjwop.html

[S03] C：读入整数
来源：http://hz.xuanzx.com/gtuuorrrnm.html

int x; scanf("%d", &x);
来源：http://hz.pycfn.com/gtbvdhyppr.html

[S04] C：字符串复制
来源：http://hz.cheryme.top/gtqscwnuww.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.daria6918.cn/gtrcqhrwrc.html

[S05] C：字符串长度
来源：http://hz.guowangkeji.top/gteljwzrvn.html

strlen(s)
来源：http://hz.hfpthk.cn/gtrvurzatm.html

[S06] C：字符串比较
来源：http://hz.ppjwa.cn/gtiwxxxica.html

strcmp(a, b) == 0
来源：http://hz.zhongyouzk.top/gthlrfrksu.html

[S07] C：数组遍历求和
来源：http://hz.c1oappe.top/gtiekbnaxi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.daria6918.cn/gtfcecslqn.html

[S08] C：动态内存分配与释放
来源：http://hz.svipenyu.cn/gtpeyylwob.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.haohaochexian.top/gtwuhugrrm.html

[S09] C：结构体定义与初始化
来源：http://hz.shanyushiyangtech.top/gtmsxtqopy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.gzhubu.top/gttovmvujt.html

[S10] C：指针与解引用
来源：http://hz.xuanzx.com/gtcmhwqlkt.html

int *p = &a;  *p = 5;
来源：http://hz.yj20258888.top/gtimmxwfdj.html

[S11] C：逐行读文件
来源：http://hz.xingfuxueyuan.xyz/gthdapnqrz.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ppjwa.cn/gtpeqhpgjm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.wangdashe.top/gtflmjdddm.html

fclose(f);
来源：http://hz.shangyingyoupin.top/gtonmdvfvu.html

[S12] C：写文件
来源：http://hz.ydzc1.top/gtgoozdetm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.gotoacloud.top/gtvrhczlsf.html

[S13] C：宏定义
来源：http://hz.cdnleiting.top/gtobqevsfy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.sysykeji.top/gtmemmaimr.html

[S14] C：枚举
来源：http://hz.yj20258888.top/gtfnmkboit.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yangfankeji.com/gtjosgaimf.html

[S15] C：类型转换
来源：http://hz.tanke756.top/gtsyfywior.html

(double) a / b
来源：http://hz.chenzaomai.com/gtsrxkyizz.html

[S16] C：位操作置位
来源：http://hz.yangfankeji.com/gtvwidjuwf.html

x |= (1 << 3);
来源：http://hz.gzhubu.top/gtfudfciyw.html

[S17] C：安全拼接字符串
来源：http://hz.yangfankeji.com/gtwmcuhqmr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.guannengcc.top/gtjgnenaui.html

[S18] C：命令行参数
来源：http://hz.hfpthk.cn/gtajipjgzt.html

int main(int argc, char **argv)
来源：http://hz.jinyuanbaomall.cn/gthtbyxrjz.html

[S19] C：快速排序
来源：http://hz.snrcjt.cn/gtrjrycjva.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shanyushiyangkeji.top/gtrehogalu.html

[S20] C：二分查找
来源：http://hz.vqdsnc.cn/gtjeydroyo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.chenzaomai.com/gtrmxgsoir.html

[S21] C：字符类别判断
来源：http://hz.mhx1999.top/gtjuzkwqus.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.guowangkeji.top/gtsrhwdpvy.html

[S22] C：字符串转数字
来源：http://hz.jiagoushi.top/gtakxgqyyj.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.pycfn.com/gtdtbaeuqd.html

[S23] C：随机数
来源：http://hz.fzhhl.top/gtaxpvlpyi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hnqzz.top/gtqfxxbvwo.html

[S24] C：获取本地时间
来源：http://hz.jianghu66.top/gtkqojwxnl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.bjfxy.top/gtllpmplwk.html

[S25] C：内存拷贝
来源：http://hz.andypj.xyz/gtwtwepzvu.html

memcpy(dst, src, n);
来源：http://hz.ydzc1.top/gtkvjnxrma.html

[S26] C：内存清零
来源：http://hz.bjfxy.top/gtmgderlli.html

memset(a, 0, sizeof a);
来源：http://hz.tanke756.top/gtmmnhziky.html

[S27] C：定义常量
来源：http://hz.iojbl.cn/gtjpzanfyz.html

const double PI = 3.14159;
来源：http://hz.xuetiantiany.cn/gtmbtosdkx.html

[S28] C：静态变量
来源：http://hz.zhijiandao.cn/gtseumrqnf.html

static int counter = 0;
来源：http://hz.xinyue.icu/gtczutbgep.html

[S29] C：变参函数
来源：http://hz.cheryme.top/gtktlmbppa.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhengqikj.top/gtlujasjia.html

[S30] C：头文件保护
来源：http://hz.aizwys.cn/gtgmkwufjm.html

#ifndef X_H
来源：http://hz.daxiang520.top/gtprgeattp.html

#define X_H
来源：http://hz.tanke756.top/gtqbpnwclr.html

#endif
来源：http://hz.zdqjudy.top/gtgjaanodh.html

[S31] C++：Hello World
来源：http://hz.ydjk.org.cn/gtiwmzveiv.html

#include <iostream>
来源：http://hz.xylfe.cn/gtxwiynqdk.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.sufxvd.cn/gtvffduqau.html

[S32] C++：字符串
来源：http://hz.shuidangran.top/gtbounismy.html

std::string s = "hi";  s += "!";
来源：http://hz.ybcxt.top/gttmykhiql.html

[S33] C++：vector 增删
来源：http://hz.yvedp.cn/gtrmsxbajr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ywan-chungtsiang.top/gtrjgkvzxp.html

[S34] C++：遍历 vector
来源：http://hz.ehwqpu.com/gtpdcxhkik.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jqgfzy.top/gtuatrvjjp.html

[S35] C++：map
来源：http://hz.zhongyouzk.top/gtmdkuuwby.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yvedp.cn/gtqbbwkcuy.html

[S36] C++：unordered_map
来源：http://hz.shanyushiyangkeji.top/gtwirtdktb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xuetiantiany.cn/gtuaocranl.html

[S37] C++：set
来源：http://hz.yj20258888.top/gtgpsknbhm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jlsjyb.cn/gtwzpysypm.html

[S38] C++：排序
来源：http://hz.52xcode.cn/gtyvgelyoi.html

std::sort(v.begin(), v.end());
来源：http://hz.tian-w.cn/gtyrrugmuw.html

[S39] C++：自定义比较器排序
来源：http://hz.bjfxy.top/gtqnrplcky.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.xziqi.cn/gtxzdatuzs.html

[S40] C++：查找元素
来源：http://hz.chenjidiqi.icu/gttnyotovh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.andypj.xyz/gtpbaexnbo.html

[S41] C++：类与构造函数
来源：http://hz.cucudq.cn/gtwmtflmqs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.sysykeji.top/gtpeslkjeo.html

[S42] C++：继承与虚函数
来源：http://hz.tian-w.cn/gtflyyssmh.html

class B : public Base { public: void f() override {} };
来源：http://hz.dianchejie.cn/gtwvoyvhss.html

[S43] C++：智能指针
来源：http://hz.hongshengwenyu.top/gtjvfrfegi.html

auto p = std::make_unique<int>(5);
来源：http://hz.kuanghao11.cn/gtiogglvrj.html

[S44] C++：引用传参
来源：http://hz.daxiang520.top/gtcoivbdvn.html

void inc(int &x) { ++x; }
来源：http://hz.cdnleiting.top/gtcbckbaaf.html

[S45] C++：lambda
来源：http://hz.yj202588.top/gtluyjqast.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.gzhubu.top/gtbmnhovxx.html

[S46] C++：函数模板
来源：http://hz.yvedp.cn/gtatuegbzf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.gaohongyu789.top/gtkikxfzbw.html

[S47] C++：结构化绑定遍历
来源：http://hz.bjfxy.top/gtuybgjaiw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jlsjyb.cn/gtguggcsmj.html

[S48] C++：逐行读文件
来源：http://hz.hysaishi.cn/gtakzlnekq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.vqdsnc.cn/gtmuozrnnc.html

while (std::getline(in, line)) { }
来源：http://hz.jyoumei.cn/gtrthhgwax.html

[S49] C++：写文件
来源：http://hz.xinyue.icu/gtrdviqirw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.snrcjt.cn/gtmubovkzi.html

[S50] C++：格式化数字
来源：http://hz.zhengqikj.top/gtmqkzgqqe.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.nanxinkj.top/gttdfqevjd.html

[S51] C++：显式类型转换
来源：http://hz.xingfuxueyuan.xyz/gtrqucsupr.html

static_cast<double>(a) / b
来源：http://hz.havefunace.top/gtyutlyfrx.html

[S52] C++：const 与 noexcept
来源：http://hz.jiagoushi.top/gtpmgzznih.html

int size() const noexcept { return n_; }
来源：http://hz.jqgfzy.top/gtbnnvsbbo.html

[S53] C++：移动语义
来源：http://hz.dianchejie.cn/gtjrtmryzi.html

std::vector<int> w = std::move(v);
来源：http://hz.gotoacloud.top/gtlukxezdu.html

[S54] C++：异常处理
来源：http://hz.svipenyu.cn/gtjtowbuqj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yanxiufei.cn/gtshtmxfqx.html

[S55] C++：结构化绑定
来源：http://hz.xylfe.cn/gtzjvxduoo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.mhx1999.top/gthylfpoye.html

[S56] C++：optional
来源：http://hz.hnxiangtu.top/gttmsktwjz.html


<!-- 参考信息 -->