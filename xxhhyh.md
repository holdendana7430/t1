代发 wailian999

[Q86] 读取 JSON 字段
来源：http://hz.jqgfzy.top/gteygmhwkh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.pengpengdd.cyou/gtchhvotdb.html

[Q87] JSON 字段做条件
来源：http://hz.shanyushiyangtech.top/gtabdynngl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.shanyushiyangkeji.top/gtxpcrlvxq.html

[Q88] 行转列（条件聚合）
来源：http://hz.dianchejie.cn/gtvcivgnat.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.dianchejie.cn/gtexapdsqo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zycfv.cn/gteioftspr.html

[Q89] 判断表是否存在
来源：http://hz.zhoulong.xyz/gtjpnoaqlu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhengqikj.top/gtzzmbmewd.html

[Q90] 生成序号列
来源：http://hz.ybcxt.top/gtpdxqnjho.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.nanxuanxn.top/gtkpjcvcvh.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtelauuqxw.html

R. Bash 专题
来源：http://hz.quarkkingdee.top/gtnjyvfvok.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtnyuhmfse.html

[R01] shebang 与严格模式
来源：http://hz.xziqi.cn/gtwrznueub.html

#!/usr/bin/env bash
来源：http://hz.sufxvd.cn/gthsozoohk.html

set -euo pipefail
来源：http://hz.cashguo.top/gtqlmohcyq.html

[R02] 变量赋值与使用
来源：http://hz.redwolf501.top/gtfsqhgeoz.html

name="Tom"; echo "$name"
来源：http://hz.chenlongwang.top/gtetexqpau.html

[R03] 只读变量
来源：http://hz.chenlongwang.top/gtztnbwbro.html

readonly PI=3.14
来源：http://hz.316326.xyz/gtudgqsuvw.html

[R04] 位置参数
来源：http://hz.guannengcc.top/gtsjudotwj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.pengpengdd.cyou/gtxyymyzdz.html

[R05] 参数默认值
来源：http://hz.zhengqikj.top/gtynoeziod.html

name="${1:-default}"
来源：http://hz.jinqigufen.top/gtxyzvgyhn.html

[R06] 判断命令是否存在
来源：http://hz.havefunace.top/gtghysmzwp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.wangshuangyany.cn/gtnuvhnunw.html

[R07] if 判断文件
来源：http://hz.jinqigfzy.top/gtqtlnlxzv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xinyue.icu/gtialyyicv.html

[R08] 数值比较
来源：http://hz.kuanghao11.cn/gtbknmwwsj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ydjk.org.cn/gtxzwvivxn.html

[R09] 字符串比较
来源：http://hz.hywenlv.cn/gtwwastnep.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.birdmap.top/gtptyzqgqc.html

[R10] 正则匹配
来源：http://hz.mhx1999.top/gtkxjcdify.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.nanxinkj.top/gtmmjzedlf.html

[R11] case 多分支
来源：http://hz.sufxvd.cn/gtvsjazaoy.html

case "$1" in
来源：http://hz.yueranfly.top/gtoulipouz.html

start) echo "启动" ;;
来源：http://hz.52xcode.cn/gtrwbkqumb.html

stop)  echo "停止" ;;
来源：http://hz.yj20258888.top/gtydqubxms.html

*)     echo "未知命令" ;;
来源：http://hz.guowangkeji.top/gtseqfpsfy.html

esac
来源：http://hz.ivvv.top/gtjmdtrvrs.html

[R12] for 遍历文件
来源：http://hz.pengpengdd.cyou/gtpfjbodrd.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hfpthk.cn/gtwxkwotcj.html

[R13] for 计数循环
来源：http://hz.cucudq.cn/gtkumvfzym.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.guannengcc.top/gtuyhtxdtw.html

[R14] C 风格 for
来源：http://hz.ydjk.org.cn/gthtmkgelu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.52xcode.cn/gtktrtyuvr.html

[R15] while 逐行读文件
来源：http://hz.shuidangran.top/gtrhcpeghs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hnxiangtu.top/gtwccpapya.html

[R16] until 等待条件
来源：http://hz.sxryk.cn/gtyohqsvxh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.guannengcc.top/gttyrqzaly.html

[R17] 数组定义与取值
来源：http://hz.guannengcc.top/gtdgsvibvk.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xylfe.cn/gtavijlsyz.html

[R18] 遍历数组
来源：http://hz.gaohongyu789.top/gtsdqiyfec.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.9152youxi.cn/gtakpsysrd.html

[R19] 数组长度
来源：http://hz.hnqzz.top/gtcrvhmutm.html

echo "${#arr[@]}"
来源：http://hz.jianghu66.top/gtufkoixab.html

[R20] 关联数组（字典）
来源：http://hz.yanxiufei.cn/gtisfcaali.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ywan-chungtsiang.top/gteojbdbsj.html

[R21] 字符串长度
来源：http://hz.nanxinkj.top/gtjzjvkapp.html

echo "${#s}"
来源：http://hz.haohaochexian.top/gtoifyuwwz.html

[R22] 截取子串
来源：http://hz.gzhubu.top/gtpmbipmbl.html

echo "${s:0:5}"
来源：http://hz.mhx1999.top/gtzbujjblt.html

[R23] 字符串替换
来源：http://hz.yonumen.top/gtioguajnh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yj20258888.top/gtdlpyjojv.html

[R24] 大小写转换
来源：http://hz.yj20258888.top/gtmjjzjftn.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ywan-chungtsiang.top/gtcxfuegpw.html

[R25] 去后缀 / 去前缀
来源：http://hz.gaohongyu789.top/gtrmtcqtub.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.quarkkingdee.top/gtjmbpphpq.html

[R26] 命令替换
来源：http://hz.daxiang520.top/gtnwttxagx.html

now=$(date +%F); echo "$now"
来源：http://hz.hammf.cn/gtvtjaeosu.html

[R27] 算术展开
来源：http://hz.yonumen.top/gtkfkikfnm.html

echo $((1 + 2 * 3))
来源：http://hz.xinyue.icu/gtdduywblj.html

[R28] 浮点运算
来源：http://hz.sxryk.cn/gtwavnqqkc.html

echo "scale=2; 10/3" | bc
来源：http://hz.yanxiufei.cn/gtrwzzsiks.html

[R29] 定义函数
来源：http://hz.jqgfzy.top/gtqokhrreo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hnqzz.top/gtymqtxmvy.html

[R30] 函数返回状态码
来源：http://hz.zhijiandao.cn/gtupksnika.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.daria6918.cn/gtogbbaghe.html

[R31] 局部变量
来源：http://hz.yongpay.top/gtjcvowfeq.html

f() { local x=1; echo "$x"; }
来源：http://hz.redwolf501.top/gtmqclqvfk.html

[R32] 参数个数校验
来源：http://hz.shzxlz.cn/gtludyccvi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.havefunace.top/gtcadxjxwz.html

[R33] 捕获错误并提示行号
来源：http://hz.jinqigufen.top/gtajaxayel.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jinqigfzy.top/gtqkfhvopk.html

[R34] 退出时清理
来源：http://hz.fzhhl.top/gtjqmyaota.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yuxming.cn/gtmddcbuib.html

[R35] 后台执行并等待
来源：http://hz.xingfuxueyuan.xyz/gtmstudkbo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ydjk.org.cn/gtypdowpkp.html

[R36] 并发执行多个任务
来源：http://hz.chenlongwang.top/gtfphsxlem.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.chenjidiqi.icu/gtyrtbcbzs.html

[R37] 把输出赋给变量
来源：http://hz.wangdashe.top/gtwsdterli.html

files=$(ls -1)
来源：http://hz.hongshengwenyu.top/gtkfhrqxff.html

[R38] 管道串联
来源：http://hz.cheryme.top/gtiherauqq.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hnqzz.top/gtlbyboobv.html

[R39] 重定向标准输出与错误
来源：http://hz.cqqwz.cn/gtnsmntwop.html

cmd > out.log 2>&1
来源：http://hz.kuanghao11.cn/gtjollkzvk.html

[R40] 追加写日志
来源：http://hz.cheryme.top/gtauwutmbn.html

echo "log" >> out.log
来源：http://hz.haohaochexian.top/gtvifhiqte.html

[R41] 丢弃输出
来源：http://hz.sxryk.cn/gtnhxxsusq.html

cmd >/dev/null 2>&1
来源：http://hz.haohaochexian.top/gtkbwwjmem.html

[R42] 输入重定向
来源：http://hz.ybcxt.top/gtkdbwwgve.html

wc -l < a.txt
来源：http://hz.sxryk.cn/gtesogajnc.html

[R43] 按名字查找文件
来源：http://hz.gzhubu.top/gtqfmnfjxb.html

find . -name "*.log" -type f
来源：http://hz.jinyuanbaomall.cn/gtocnjalvb.html

[R44] 按修改时间查找
来源：http://hz.feifeiyinyue.top/gteknhvyso.html

find . -mtime -7 -type f
来源：http://hz.cucudq.cn/gtpitkjtbc.html

[R45] 批量删除
来源：http://hz.ywan-chungtsiang.top/gtyscoyyec.html

find . -name "*.tmp" -delete
来源：http://hz.zhiwuduotai.top/gtnvjbpdjr.html

[R46] 递归替换文件内容
来源：http://hz.cdnleiting.top/gtvecmdjwk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ybcxt.top/gtouqaftfd.html

[R47] sed 单行替换
来源：http://hz.pengpengdd.cyou/gtssmmssov.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhongyouzk.top/gtytzqhlqj.html

[R48] awk 取指定列
来源：http://hz.snrcjt.cn/gtdiyucpzq.html

awk '{print $1, $3}' a.txt
来源：http://hz.meibo888.top/gtkujdzjby.html

[R49] awk 带条件
来源：http://hz.ydzc1.top/gtmljbkcag.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.sweek.top/gtjzxybjxk.html

[R50] awk 求和
来源：http://hz.jinqigfzy.top/gtaowqnsuw.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zycfv.cn/gtnloyokph.html

[R51] 排序去重取前几
来源：http://hz.gogol.net.cn/gtlqcmkpid.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.fzhhl.top/gtxzljqrtr.html

[R52] 统计行数
来源：http://hz.jinqigufen.top/gtrbeafvgr.html

wc -l a.txt
来源：http://hz.havefunace.top/gtkjcwdhqw.html

[R53] 查看文件头与实时尾
来源：http://hz.aibaodan.cn/gttpprphto.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.nanxinkj.top/gthftxnbhs.html

[R54] 比较两个文件
来源：http://hz.sweek.top/gtpnmwxeva.html

diff a.txt b.txt
来源：http://hz.yuanzhike.top/gtwfblmcvj.html

[R55] 压缩与解压
来源：http://hz.yangfankeji.com/gtubiftaes.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jiagoushi.top/gtiumdzsrg.html

[R56] 远程拷贝
来源：http://hz.gogol.net.cn/gthzjvthdj.html

scp file user@host:/path/
来源：http://hz.hywenlv.cn/gtdgghpqmg.html

[R57] 远程执行命令
来源：http://hz.tanke756.top/gtcgghizlx.html

ssh user@host 'uptime'
来源：http://hz.guannengcc.top/gtcennkuos.html

[R58] 下载文件
来源：http://hz.hnxiangtu.top/gteowjiifz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yj202588.top/gtjofozolm.html

[R59] 发 POST JSON
来源：http://hz.nanxinkj.top/gtbqvdlcfc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yuxming.cn/gtyplczhdr.html

[R60] 只看 HTTP 状态码
来源：http://hz.wangshuangyany.cn/gteequpahz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhixingplan.top/gtxrkyaupm.html

[R61] 磁盘占用
来源：http://hz.hnqzz.top/gtdxapasej.html

df -h;  du -sh *
来源：http://hz.aizwys.cn/gtabpfjfbj.html

[R62] 找最占空间的文件
来源：http://hz.xylfe.cn/gtljbzrqda.html

du -ah . | sort -rh | head -10
来源：http://hz.bjfxy.top/gtbyhimfzg.html

[R63] 内存与进程
来源：http://hz.ydjk.org.cn/gtpjwcmzjo.html

free -h;  ps aux | grep nginx
来源：http://hz.iojbl.cn/gtlrkfcohg.html

[R64] 结束进程
来源：http://hz.yuxming.cn/gtrzskdgmw.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yj20258.top/gtfvkmhdcl.html

[R65] 查看端口占用
来源：http://hz.snrcjt.cn/gtjpurqcbg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.cdnleiting.top/gtieycvils.html

[R66] 定时任务
来源：http://hz.chenlongwang.top/gttjcguhbi.html

crontab -e;  crontab -l
来源：http://hz.svipenyu.cn/gthggiiffn.html

[R67] 生成随机十六进制串
来源：http://hz.gzhubu.top/gtkvqeqrsg.html

openssl rand -hex 16
来源：http://hz.cheryme.top/gtkktbwkcs.html

[R68] 计算文件校验值
来源：http://hz.svipenyu.cn/gtpvqtnwbg.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.daxiang520.top/gtghewynzn.html

[R69] 生成随机密码
来源：http://hz.pycfn.com/gtdjpmshbx.html

head -c 16 /dev/urandom | base64
来源：http://hz.shanyushiyangtech.top/gtgbpgveny.html

[R70] 时间戳与互转
来源：http://hz.ivvv.top/gtoouwjlhs.html

date +%s;  date -d @1700000000
来源：http://hz.52xcode.cn/gtbmaoqams.html

[R71] 日期格式化
来源：http://hz.gogol.net.cn/gtapeijbhx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.pycfn.com/gthdomzmys.html

[R72] 等待端口就绪
来源：http://hz.shangyingyoupin.top/gtghfffyct.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hnqzz.top/gtecihfwde.html

[R73] 分割大日志
来源：http://hz.xuetiantiany.cn/gtoczlnwwm.html

split -l 1000 big.log part_
来源：http://hz.52xcode.cn/gtchaxwfxn.html

[R74] 批量重命名
来源：http://hz.52xcode.cn/gtlxyyucgz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.shanyushiyangtech.top/gtqltuxdwo.html

[R75] 导出环境变量
来源：http://hz.aibaodan.cn/gtrvuwmvou.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jiagoushi.top/gtcppizinl.html

[R76] 使用临时文件
来源：http://hz.jinqigfzy.top/gtqqzqmkzv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.redwolf501.top/gtevlwediy.html

[R77] 读取用户输入
来源：http://hz.shanyushiyangtech.top/gtjgoioglw.html

read -rp "请输入: " ans
来源：http://hz.redwolf501.top/gtrgajxpmy.html

[R78] 交互式菜单
来源：http://hz.52xcode.cn/gtnjlgnjzq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.birdmap.top/gtxxemdzdg.html

[R79] 解析命令行选项
来源：http://hz.hnxiangtu.top/gtjrkedkwm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.gotoacloud.top/gtkrfjscdv.html

[R80] 查看脚本执行耗时
来源：http://hz.xuanzx.com/gtzvtgvvmc.html

time ./run.sh
来源：http://hz.ybcxt.top/gtgnptreof.html

================================================================================
来源：http://hz.ybcxt.top/gtgklkmzdb.html

S. C / C++ 专题
来源：http://hz.smart0.xyz/gtbrowtyez.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtqazefpig.html

[S01] C：Hello World
来源：http://hz.zhiwuduotai.top/gtmcxninnz.html

#include <stdio.h>
来源：http://hz.sweek.top/gtyfvgsvde.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xziqi.cn/gtblylzbtw.html

[S02] C：变量与格式化输出
来源：http://hz.yj202588.top/gtjqlaleku.html

int a = 10; printf("%d\n", a);
来源：http://hz.sysykeji.top/gttijruftn.html

[S03] C：读入整数
来源：http://hz.yueranfly.top/gtjcwdvewa.html

int x; scanf("%d", &x);
来源：http://hz.tanke756.top/gtqufnnytq.html

[S04] C：字符串复制
来源：http://hz.jqgufenzy.top/gttyckwycs.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.redwolf501.top/gtiqfxvdqs.html

[S05] C：字符串长度
来源：http://hz.tanke756.top/gthbcqkvrn.html

strlen(s)
来源：http://hz.jianghu66.top/gtikeldlqv.html

[S06] C：字符串比较
来源：http://hz.gogol.net.cn/gtitksraep.html

strcmp(a, b) == 0
来源：http://hz.zdqjudy.top/gtootdzsdo.html

[S07] C：数组遍历求和
来源：http://hz.316326.xyz/gtcmflyuop.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.dianchejie.cn/gtlexkmrxi.html

[S08] C：动态内存分配与释放
来源：http://hz.ydzc1.top/gtcrhrcygb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yonumen.top/gtirlaggmg.html

[S09] C：结构体定义与初始化
来源：http://hz.dashuyun.cn/gtfewaiwdl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yueranfly.top/gtqhonlltb.html

[S10] C：指针与解引用
来源：http://hz.ehwqpu.com/gtbchixclq.html

int *p = &a;  *p = 5;
来源：http://hz.ybcxt.top/gtdlzfgtjc.html

[S11] C：逐行读文件
来源：http://hz.tianlin.xyz/gtmqwutrha.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jinqigfzy.top/gtjhalustf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.feifeiyinyue.top/gtvyrjqkhu.html

fclose(f);
来源：http://hz.xuanzx.com/gtrkbdvtfi.html

[S12] C：写文件
来源：http://hz.haohaochexian.top/gtuksmfuuh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ppjwa.cn/gtigfmnqew.html

[S13] C：宏定义
来源：http://hz.ydjk.org.cn/gtynieccoq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.nanxuanxn.top/gtuhhqgpoz.html

[S14] C：枚举
来源：http://hz.daxiang520.top/gtrwyczasn.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.tanke756.top/gtzgdtogwp.html

[S15] C：类型转换
来源：http://hz.zycfv.cn/gtfhvaibcv.html

(double) a / b
来源：http://hz.zhijiandao.cn/gtlsvglgvo.html

[S16] C：位操作置位
来源：http://hz.gaohongyu789.top/gtbayjyhqt.html

x |= (1 << 3);
来源：http://hz.haohaochexian.top/gtxakplyzc.html

[S17] C：安全拼接字符串
来源：http://hz.tanke756.top/gtsnytpdjz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.dianchejie.cn/gtxlkdjxho.html

[S18] C：命令行参数
来源：http://hz.wangshuangyany.cn/gtugckyfqo.html

int main(int argc, char **argv)
来源：http://hz.cqqwz.cn/gtgpcgeqvp.html

[S19] C：快速排序
来源：http://hz.ydjk.org.cn/gthfawjjuf.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hysaishi.cn/gtwuwsxphq.html

[S20] C：二分查找
来源：http://hz.yj202588.top/gtmitrnnst.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.kuanghao11.cn/gtydvwveqv.html

[S21] C：字符类别判断
来源：http://hz.tianlin.xyz/gtmocoobkw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jqgufenzy.top/gtfsyypxul.html

[S22] C：字符串转数字
来源：http://hz.ehwqpu.com/gtphjkxzmx.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.smart0.xyz/gthzvuusjs.html

[S23] C：随机数
来源：http://hz.zhoulong.xyz/gtadhsezng.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zdqjudy.top/gtibutvjkd.html

[S24] C：获取本地时间
来源：http://hz.cashguo.top/gtzjkqqozi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.birdmap.top/gtqrihhkzq.html

[S25] C：内存拷贝
来源：http://hz.hywenlv.cn/gtjwufbita.html

memcpy(dst, src, n);
来源：http://hz.guannengcc.top/gtbfhtejil.html

[S26] C：内存清零
来源：http://hz.jyoumei.cn/gtpkynedzy.html

memset(a, 0, sizeof a);
来源：http://hz.jqgufenzy.top/gtbewgmhjz.html

[S27] C：定义常量
来源：http://hz.yangfankeji.com/gtybexnpfc.html

const double PI = 3.14159;
来源：http://hz.wangshuangyany.cn/gtlxcggzdu.html

[S28] C：静态变量
来源：http://hz.feifeiyinyue.top/gtdxrjsdtu.html

static int counter = 0;
来源：http://hz.cqqwz.cn/gtjevftowo.html

[S29] C：变参函数
来源：http://hz.andypj.xyz/gtprkchrpk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cheryme.top/gtmftjirvb.html

[S30] C：头文件保护
来源：http://hz.xingfuxueyuan.xyz/gtxreepfva.html

#ifndef X_H
来源：http://hz.jiagoushi.top/gtoktujsot.html

#define X_H
来源：http://hz.xuetiantiany.cn/gtfigwyxdu.html

#endif
来源：http://hz.redwolf501.top/gtnhhjcalq.html

[S31] C++：Hello World
来源：http://hz.9152youxi.cn/gtmtbkfdlt.html

#include <iostream>
来源：http://hz.yonumen.top/gtbckeaueg.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.shanyushiyangtech.top/gtuaofpebr.html

[S32] C++：字符串
来源：http://hz.chenjidiqi.icu/gtunwglvzr.html

std::string s = "hi";  s += "!";
来源：http://hz.jinqigfzy.top/gtzhaoyoqw.html

[S33] C++：vector 增删
来源：http://hz.c1oappe.top/gttumtmlpk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xuetiantiany.cn/gtfikgnkhs.html

[S34] C++：遍历 vector
来源：http://hz.zhijiandao.cn/gtxkqgihgm.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yj20258.top/gtwludjkim.html

[S35] C++：map
来源：http://hz.zhongyouzk.top/gtwfzkknmt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shangyingyoupin.top/gtrfwqxiai.html

[S36] C++：unordered_map
来源：http://hz.dashuyun.cn/gtjcxrrfwd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.quarkkingdee.top/gtrqegilwz.html

[S37] C++：set
来源：http://hz.zhengqikj.top/gtfwxmprxf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yueranfly.top/gtteznlnxv.html

[S38] C++：排序
来源：http://hz.sysykeji.top/gtjywesjuj.html

std::sort(v.begin(), v.end());
来源：http://hz.nanxuanxn.top/gtahhrugjm.html

[S39] C++：自定义比较器排序
来源：http://hz.chenlongwang.top/gtjkcrfmeh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.sysykeji.top/gtsfieqjmr.html

[S40] C++：查找元素
来源：http://hz.kuanghao11.cn/gtjwpmrzhw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.andypj.xyz/gtjmqmiqeh.html

[S41] C++：类与构造函数
来源：http://hz.xuanzx.com/gtjnofktgy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yuanzhike.top/gtonsnaoyt.html

[S42] C++：继承与虚函数
来源：http://hz.andypj.xyz/gtqeiqrxzu.html

class B : public Base { public: void f() override {} };
来源：http://hz.yanxiufei.cn/gtmvgjgzuk.html

[S43] C++：智能指针
来源：http://hz.zhijiandao.cn/gtluaokaxv.html

auto p = std::make_unique<int>(5);
来源：http://hz.bjfxy.top/gtlpiudztd.html

[S44] C++：引用传参
来源：http://hz.meibo888.top/gtmagwrwlb.html

void inc(int &x) { ++x; }
来源：http://hz.hnqzz.top/gtdfepnabg.html

[S45] C++：lambda
来源：http://hz.yangfankeji.com/gtzscyldlp.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cdnleiting.top/gtdxfowymo.html

[S46] C++：函数模板
来源：http://hz.zhiwuduotai.top/gtzrvveuvm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.cqqwz.cn/gtgozgtxle.html

[S47] C++：结构化绑定遍历
来源：http://hz.chenjidiqi.icu/gtcqgmolai.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ybcxt.top/gtzyudoywb.html

[S48] C++：逐行读文件
来源：http://hz.pengpengdd.cyou/gtqhgziwig.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.chenlongwang.top/gtuhdkcrkr.html

while (std::getline(in, line)) { }
来源：http://hz.yj20258.top/gtlafoifuh.html

[S49] C++：写文件
来源：http://hz.sweek.top/gtetymjcdc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.bjfxy.top/gtvhyxluih.html

[S50] C++：格式化数字
来源：http://hz.jqgfzy.top/gtwtmzggvp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.iojbl.cn/gttnoaacud.html

[S51] C++：显式类型转换
来源：http://hz.yj20258888.top/gtmoalamqc.html

static_cast<double>(a) / b
来源：http://hz.tianlin.xyz/gtiiwpwgul.html

[S52] C++：const 与 noexcept
来源：http://hz.jyoumei.cn/gtwvujpvje.html

int size() const noexcept { return n_; }
来源：http://hz.shanyushiyangkeji.top/gtsavuxypw.html

[S53] C++：移动语义
来源：http://hz.yj202588.top/gtlawhwazp.html

std::vector<int> w = std::move(v);
来源：http://hz.guannengcc.top/gtjgnblkhf.html

[S54] C++：异常处理
来源：http://hz.guowangkeji.top/gtpbgswehg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.shanyushiyangtech.top/gtjvvkkbgg.html

[S55] C++：结构化绑定
来源：http://hz.yonumen.top/gtjvosbahk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.aizwys.cn/gtymbczxpz.html

[S56] C++：optional
来源：http://hz.ydjk.org.cn/gtjcqacpbg.html


<!-- 参考信息 -->