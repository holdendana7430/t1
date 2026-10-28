代发 wailian999

[Q82] 字符长度与字节长度
来源：http://hz.chenjidiqi.icu/gthuhpcijp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtwnnychsg.html

[Q83] 大小写转换
来源：http://hz.iojbl.cn/gtzmlssfhf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hysaishi.cn/gtazhsgwju.html

[Q84] 去除首尾空格
来源：http://hz.smart0.xyz/gtbnoubgxf.html

SELECT TRIM(name) FROM users;
来源：http://hz.jlsjyb.cn/gtqfzwrxep.html

[Q85] 数值取整
来源：http://hz.zycfv.cn/gtbyprumcw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cheryme.top/gtaprhuetb.html

[Q86] 读取 JSON 字段
来源：http://hz.zhijiandao.cn/gtntakkrzj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.wangshuangyany.cn/gtoahsfagj.html

[Q87] JSON 字段做条件
来源：http://hz.yangfankeji.com/gtifjgbzhy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.pycfn.com/gtxfcgikzg.html

[Q88] 行转列（条件聚合）
来源：http://hz.cdnleiting.top/gtljjpjckw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hnxiangtu.top/gtwiqyagck.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.andypj.xyz/gtrkjgthds.html

[Q89] 判断表是否存在
来源：http://hz.zycfv.cn/gtbhzasdxi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.guannengcc.top/gtehykxmhg.html

[Q90] 生成序号列
来源：http://hz.dianchejie.cn/gtwvbluoks.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.feifeiyinyue.top/gtdtpwbfwe.html

================================================================================
来源：http://hz.aizwys.cn/gtfbhgyzqn.html

R. Bash 专题
来源：http://hz.hywenlv.cn/gtcesqdruq.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtifcjouoq.html

[R01] shebang 与严格模式
来源：http://hz.ybcxt.top/gtlgwsxnwy.html

#!/usr/bin/env bash
来源：http://hz.daria6918.cn/gttlqxjbud.html

set -euo pipefail
来源：http://hz.shuidangran.top/gtzkctzaru.html

[R02] 变量赋值与使用
来源：http://hz.hongshengwenyu.top/gtjcuctbzs.html

name="Tom"; echo "$name"
来源：http://hz.meibo888.top/gtpuuarmjp.html

[R03] 只读变量
来源：http://hz.c1oappe.top/gtzlkcdsxv.html

readonly PI=3.14
来源：http://hz.xuetiantiany.cn/gtsuvewatb.html

[R04] 位置参数
来源：http://hz.jqgfzy.top/gtjjywakqx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.chenlongwang.top/gthdsxrsly.html

[R05] 参数默认值
来源：http://hz.feifeiyinyue.top/gtbtmxllyo.html

name="${1:-default}"
来源：http://hz.hysaishi.cn/gtdqwpabdu.html

[R06] 判断命令是否存在
来源：http://hz.shanyushiyangtech.top/gtupzsppqd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.0kj1m.cn/gtedlrkonr.html

[R07] if 判断文件
来源：http://hz.yanxiufei.cn/gthdmfpwqs.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yuxming.cn/gtmscnyavd.html

[R08] 数值比较
来源：http://hz.hywenlv.cn/gtikfcmszl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shanyushiyangtech.top/gthqmkjkiz.html

[R09] 字符串比较
来源：http://hz.haohaochexian.top/gtbubqikgj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ywan-chungtsiang.top/gtooabzezu.html

[R10] 正则匹配
来源：http://hz.hnqzz.top/gtjxfptmva.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.xingfuxueyuan.xyz/gtvdsernhb.html

[R11] case 多分支
来源：http://hz.zycfv.cn/gtcoujfcap.html

case "$1" in
来源：http://hz.zhaomingkeji.xyz/gtxgeulppn.html

start) echo "启动" ;;
来源：http://hz.yuxming.cn/gtoklsikvn.html

stop)  echo "停止" ;;
来源：http://hz.c1oappe.top/gtcydaqthc.html

*)     echo "未知命令" ;;
来源：http://hz.chenjidiqi.icu/gtlhdfitrg.html

esac
来源：http://hz.fzhhl.top/gtpmeysszv.html

[R12] for 遍历文件
来源：http://hz.nanxinkj.top/gtgcuxhqbc.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hongshengwenyu.top/gtnfditjvw.html

[R13] for 计数循环
来源：http://hz.zhijiandao.cn/gtsfbmzlye.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.shuidangran.top/gtexfajupr.html

[R14] C 风格 for
来源：http://hz.jinyuanbaomall.cn/gtdhsctnpr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hammf.cn/gtffecolrt.html

[R15] while 逐行读文件
来源：http://hz.smart0.xyz/gtztdhrzjv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.shangyingyoupin.top/gtzjopwhfj.html

[R16] until 等待条件
来源：http://hz.aizwys.cn/gtaudoyris.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yangfankeji.com/gtelpdxhca.html

[R17] 数组定义与取值
来源：http://hz.zhaomingkeji.xyz/gtdblgiqxi.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhengqikj.top/gtlmlbomhs.html

[R18] 遍历数组
来源：http://hz.ppjwa.cn/gtaizjhbwd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xinyue.icu/gtsnrnwokq.html

[R19] 数组长度
来源：http://hz.haohaochexian.top/gtemklmrwx.html

echo "${#arr[@]}"
来源：http://hz.xylfe.cn/gtyllcsnze.html

[R20] 关联数组（字典）
来源：http://hz.pengpengdd.cyou/gtvtparype.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.0kj1m.cn/gtwmdnnhle.html

[R21] 字符串长度
来源：http://hz.ppjwa.cn/gtezgltjxm.html

echo "${#s}"
来源：http://hz.chenlongwang.top/gtdpaqqlpr.html

[R22] 截取子串
来源：http://hz.yj202588.top/gtwxwfofgj.html

echo "${s:0:5}"
来源：http://hz.pycfn.com/gtpbtxvfyd.html

[R23] 字符串替换
来源：http://hz.yj202588.top/gtumlrgxdv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yj20258888.top/gtamntfjlo.html

[R24] 大小写转换
来源：http://hz.zdqjudy.top/gtorxglxrp.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jinyuanbaomall.cn/gtrazobvlf.html

[R25] 去后缀 / 去前缀
来源：http://hz.iojbl.cn/gtnlllvobo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.wangdashe.top/gtfkujqtay.html

[R26] 命令替换
来源：http://hz.zhaomingkeji.xyz/gtvcsdfqol.html

now=$(date +%F); echo "$now"
来源：http://hz.haohaochexian.top/gtjilcgcpn.html

[R27] 算术展开
来源：http://hz.pycfn.com/gtaeznwnvs.html

echo $((1 + 2 * 3))
来源：http://hz.ehwqpu.com/gtfxowapis.html

[R28] 浮点运算
来源：http://hz.wangshuangyany.cn/gtvtpnqzmy.html

echo "scale=2; 10/3" | bc
来源：http://hz.jianghu66.top/gtgavcnmhl.html

[R29] 定义函数
来源：http://hz.dashuyun.cn/gtbhzmrwbo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.fengsongda.top/gtizumfllz.html

[R30] 函数返回状态码
来源：http://hz.guowangkeji.top/gtsqweiygk.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.shangyingyoupin.top/gtblzikvap.html

[R31] 局部变量
来源：http://hz.nanxuanxn.top/gterwibgba.html

f() { local x=1; echo "$x"; }
来源：http://hz.jqgfzy.top/gtiwjbsrkf.html

[R32] 参数个数校验
来源：http://hz.jinqigfzy.top/gtylmomcmn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.svipenyu.cn/gtoedvfpnr.html

[R33] 捕获错误并提示行号
来源：http://hz.9152youxi.cn/gtedfqicpy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shzxlz.cn/gttiaemfuu.html

[R34] 退出时清理
来源：http://hz.guowangkeji.top/gtjzikzcay.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ybcxt.top/gtlheqaevv.html

[R35] 后台执行并等待
来源：http://hz.zhongyouzk.top/gtcbjjnghg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yonumen.top/gteqpexuws.html

[R36] 并发执行多个任务
来源：http://hz.ppjwa.cn/gtdezbkgtt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ehwqpu.com/gtfpvciuym.html

[R37] 把输出赋给变量
来源：http://hz.hnqzz.top/gtodhdepgr.html

files=$(ls -1)
来源：http://hz.ydjk.org.cn/gtmdufbrru.html

[R38] 管道串联
来源：http://hz.svipenyu.cn/gtxhhntlyd.html

cat a.txt | grep -i error | wc -l
来源：http://hz.dashuyun.cn/gtrtecchfr.html

[R39] 重定向标准输出与错误
来源：http://hz.sweek.top/gtxhrbwlkz.html

cmd > out.log 2>&1
来源：http://hz.zycfv.cn/gtveihfgjo.html

[R40] 追加写日志
来源：http://hz.shuidangran.top/gtuqxeyayn.html

echo "log" >> out.log
来源：http://hz.daxiang520.top/gtfnjosafj.html

[R41] 丢弃输出
来源：http://hz.xuetiantiany.cn/gtinvucnrt.html

cmd >/dev/null 2>&1
来源：http://hz.guannengcc.top/gtflwtkwsv.html

[R42] 输入重定向
来源：http://hz.hfpthk.cn/gtkxiosegm.html

wc -l < a.txt
来源：http://hz.ybcxt.top/gtcyncqzdt.html

[R43] 按名字查找文件
来源：http://hz.zhixingplan.top/gtwfdgcodm.html

find . -name "*.log" -type f
来源：http://hz.gotoacloud.top/gtqkcjsylz.html

[R44] 按修改时间查找
来源：http://hz.mhx1999.top/gtewqqzfxm.html

find . -mtime -7 -type f
来源：http://hz.xziqi.cn/gtszdsyxdr.html

[R45] 批量删除
来源：http://hz.jianghu66.top/gtbjrqhtsz.html

find . -name "*.tmp" -delete
来源：http://hz.vqdsnc.cn/gtpfnqmojk.html

[R46] 递归替换文件内容
来源：http://hz.tanke756.top/gtwdsijwyd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.nanxuanxn.top/gtlfqkqdgg.html

[R47] sed 单行替换
来源：http://hz.zhongyouzk.top/gttikucqkw.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhiwuduotai.top/gtcrixwied.html

[R48] awk 取指定列
来源：http://hz.ppjwa.cn/gthckcfcbj.html

awk '{print $1, $3}' a.txt
来源：http://hz.ydjk.org.cn/gtyccpqvyz.html

[R49] awk 带条件
来源：http://hz.yonumen.top/gtrhqvgvdk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yanxiufei.cn/gtcgpirhig.html

[R50] awk 求和
来源：http://hz.yongpay.top/gtwkhowtws.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ppjwa.cn/gtmzrclnec.html

[R51] 排序去重取前几
来源：http://hz.gotoacloud.top/gtzwfrbqqm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhoulong.xyz/gtalhggxkn.html

[R52] 统计行数
来源：http://hz.jqgfzy.top/gtuqkmmaka.html

wc -l a.txt
来源：http://hz.shangyingyoupin.top/gthqyfgtij.html

[R53] 查看文件头与实时尾
来源：http://hz.iojbl.cn/gtpiwcxvcg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.chenlongwang.top/gtikzzdrjd.html

[R54] 比较两个文件
来源：http://hz.zhaomingkeji.xyz/gtkhhyzutq.html

diff a.txt b.txt
来源：http://hz.yangfankeji.com/gtlvpmiguc.html

[R55] 压缩与解压
来源：http://hz.daxiang520.top/gtrumubyis.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jlsjyb.cn/gtckvzrphb.html

[R56] 远程拷贝
来源：http://hz.zhengqikj.top/gtfbjayojw.html

scp file user@host:/path/
来源：http://hz.zhaomingkeji.xyz/gtxmwztcvk.html

[R57] 远程执行命令
来源：http://hz.jqgufenzy.top/gtuedsrfgl.html

ssh user@host 'uptime'
来源：http://hz.pengpengdd.cyou/gttigihccm.html

[R58] 下载文件
来源：http://hz.hnxiangtu.top/gtzejasyja.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.haohaochexian.top/gtgbfpavqa.html

[R59] 发 POST JSON
来源：http://hz.zhongyouzk.top/gtdkpvbrvg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.9152youxi.cn/gtnhnapmwr.html

[R60] 只看 HTTP 状态码
来源：http://hz.ppjwa.cn/gtpmwvvnur.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.haohaochexian.top/gtwtbpkqjv.html

[R61] 磁盘占用
来源：http://hz.gotoacloud.top/gtyqhuocwn.html

df -h;  du -sh *
来源：http://hz.xuanzx.com/gtwqdbiqlq.html

[R62] 找最占空间的文件
来源：http://hz.nanxinkj.top/gtvepvepdu.html

du -ah . | sort -rh | head -10
来源：http://hz.zhixingplan.top/gttkweevtz.html

[R63] 内存与进程
来源：http://hz.ehwqpu.com/gtedwizmit.html

free -h;  ps aux | grep nginx
来源：http://hz.pengpengdd.cyou/gtxhaylvnj.html

[R64] 结束进程
来源：http://hz.aibaodan.cn/gtpxcryoha.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hnqzz.top/gttydchaos.html

[R65] 查看端口占用
来源：http://hz.ybcxt.top/gtrgdsiswa.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jqgufenzy.top/gtbbjtquah.html

[R66] 定时任务
来源：http://hz.jinghuilouyu.cn/gtflfkvznm.html

crontab -e;  crontab -l
来源：http://hz.chenjidiqi.icu/gtnttvispp.html

[R67] 生成随机十六进制串
来源：http://hz.zhaomingkeji.xyz/gtmoqqnkpt.html

openssl rand -hex 16
来源：http://hz.pycfn.com/gtxdamelzv.html

[R68] 计算文件校验值
来源：http://hz.shuidangran.top/gtgfgdzuff.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.sxryk.cn/gtfzrovmoe.html

[R69] 生成随机密码
来源：http://hz.wangdashe.top/gticihercz.html

head -c 16 /dev/urandom | base64
来源：http://hz.ivvv.top/gtyhcqepir.html

[R70] 时间戳与互转
来源：http://hz.dashuyun.cn/gtdndvpgqi.html

date +%s;  date -d @1700000000
来源：http://hz.hysaishi.cn/gtitzjdeyn.html

[R71] 日期格式化
来源：http://hz.jinqigfzy.top/gtuztwolsn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.aizwys.cn/gtoanrfkzz.html

[R72] 等待端口就绪
来源：http://hz.jinqigfzy.top/gtkvjoecni.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.shanyushiyangkeji.top/gtojlxxaxu.html

[R73] 分割大日志
来源：http://hz.chenlongwang.top/gtpdseztcn.html

split -l 1000 big.log part_
来源：http://hz.52xcode.cn/gtgcosgbfp.html

[R74] 批量重命名
来源：http://hz.nanxinkj.top/gtwxdhhkds.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.guannengcc.top/gtvakampzr.html

[R75] 导出环境变量
来源：http://hz.wangdashe.top/gtmtwjsdgu.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yj20258.top/gtctybbmkh.html

[R76] 使用临时文件
来源：http://hz.jinqigufen.top/gtwmeskolm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yongpay.top/gtqzuuibzn.html

[R77] 读取用户输入
来源：http://hz.jqgufenzy.top/gtvxwhlvwp.html

read -rp "请输入: " ans
来源：http://hz.ehwqpu.com/gtgmmhvffj.html

[R78] 交互式菜单
来源：http://hz.gogol.net.cn/gtmwgbmija.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xinyue.icu/gtoesqlmoo.html

[R79] 解析命令行选项
来源：http://hz.havefunace.top/gtickgrwnk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xinyue.icu/gtnvrwktod.html

[R80] 查看脚本执行耗时
来源：http://hz.jianghu66.top/gtjooqajhj.html

time ./run.sh
来源：http://hz.shanyushiyangtech.top/gthjiolpij.html

================================================================================
来源：http://hz.aibaodan.cn/gtrzioynpz.html

S. C / C++ 专题
来源：http://hz.sufxvd.cn/gtrlbwwipt.html

================================================================================
来源：http://hz.yuanzhike.top/gtjppkpjof.html

[S01] C：Hello World
来源：http://hz.yangfankeji.com/gtjdzkijvt.html

#include <stdio.h>
来源：http://hz.daxiang520.top/gtjxsoravn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jinqigufen.top/gtmukqeimh.html

[S02] C：变量与格式化输出
来源：http://hz.dashuyun.cn/gtaymchkke.html

int a = 10; printf("%d\n", a);
来源：http://hz.birdmap.top/gtnplzhbzs.html

[S03] C：读入整数
来源：http://hz.ybcxt.top/gtqiyjpmfv.html

int x; scanf("%d", &x);
来源：http://hz.yuxming.cn/gtruitueot.html

[S04] C：字符串复制
来源：http://hz.cashguo.top/gtsnubdafg.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.havefunace.top/gtflzpbjje.html

[S05] C：字符串长度
来源：http://hz.chenzaomai.com/gtlyeenehj.html

strlen(s)
来源：http://hz.tianlin.xyz/gtzbcedbiu.html

[S06] C：字符串比较
来源：http://hz.sysykeji.top/gtjlzqgbpf.html

strcmp(a, b) == 0
来源：http://hz.dianchejie.cn/gtrgoanilk.html

[S07] C：数组遍历求和
来源：http://hz.birdmap.top/gtcpvatrro.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hfpthk.cn/gtcwelocrc.html

[S08] C：动态内存分配与释放
来源：http://hz.sufxvd.cn/gtunfxexra.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.vqdsnc.cn/gtaalbxcrt.html

[S09] C：结构体定义与初始化
来源：http://hz.nanxuanxn.top/gtitaammas.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ppjwa.cn/gtdzaeglgj.html

[S10] C：指针与解引用
来源：http://hz.andypj.xyz/gttnqsedch.html

int *p = &a;  *p = 5;
来源：http://hz.daria6918.cn/gtcyiunrga.html

[S11] C：逐行读文件
来源：http://hz.guowangkeji.top/gtyzvrkcya.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.xziqi.cn/gtcpochtbj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.vqdsnc.cn/gtmjnzqqos.html

fclose(f);
来源：http://hz.gotoacloud.top/gtwsjnyfoi.html

[S12] C：写文件
来源：http://hz.havefunace.top/gtltbjeuep.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.sxryk.cn/gtpmcqhccd.html

[S13] C：宏定义
来源：http://hz.andypj.xyz/gtvqnpdxnr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhiwuduotai.top/gtthbkrepu.html

[S14] C：枚举
来源：http://hz.shanyushiyangkeji.top/gtxcwylavu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zycfv.cn/gthhdrbmht.html

[S15] C：类型转换
来源：http://hz.cheryme.top/gthhtjefre.html

(double) a / b
来源：http://hz.vqdsnc.cn/gtlfpxmemb.html

[S16] C：位操作置位
来源：http://hz.aizwys.cn/gtyinmtgvf.html

x |= (1 << 3);
来源：http://hz.zdqjudy.top/gtcbmwinma.html

[S17] C：安全拼接字符串
来源：http://hz.iojbl.cn/gtusnatcpb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yj20258.top/gtxdyusipu.html

[S18] C：命令行参数
来源：http://hz.ppjwa.cn/gtxxtbdgti.html

int main(int argc, char **argv)
来源：http://hz.xylfe.cn/gtehdnehvu.html

[S19] C：快速排序
来源：http://hz.chenzaomai.com/gtgkafcdoy.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yuxming.cn/gtdlzggujx.html

[S20] C：二分查找
来源：http://hz.zhijiandao.cn/gtywjfbijz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ybcxt.top/gtakshjqay.html

[S21] C：字符类别判断
来源：http://hz.nwbrower.top/gttiducgqh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.bjfxy.top/gtidfmkfur.html

[S22] C：字符串转数字
来源：http://hz.shzxlz.cn/gtnrxqixvv.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.andypj.xyz/gtkogoozip.html

[S23] C：随机数
来源：http://hz.xuetiantiany.cn/gtmzvowdkr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.haohaochexian.top/gtakgilyyg.html

[S24] C：获取本地时间
来源：http://hz.yvedp.cn/gtlbjukpto.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.pycfn.com/gtmvmtbeex.html

[S25] C：内存拷贝
来源：http://hz.jinghuilouyu.cn/gtthorhadj.html

memcpy(dst, src, n);
来源：http://hz.zhongyouzk.top/gtpdduyjrz.html

[S26] C：内存清零
来源：http://hz.haohaochexian.top/gtemvfkugl.html

memset(a, 0, sizeof a);
来源：http://hz.jinqigfzy.top/gtdfgllovd.html

[S27] C：定义常量
来源：http://hz.chenlongwang.top/gtlckzstev.html

const double PI = 3.14159;
来源：http://hz.zhaomingkeji.xyz/gtwrayzzan.html

[S28] C：静态变量
来源：http://hz.fzhhl.top/gtxpeicnmc.html

static int counter = 0;
来源：http://hz.birdmap.top/gtmrvryhei.html

[S29] C：变参函数
来源：http://hz.andypj.xyz/gtzskddxhv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shangyingyoupin.top/gtvdiuipwu.html

[S30] C：头文件保护
来源：http://hz.jinghuilouyu.cn/gtsxjlmtbz.html

#ifndef X_H
来源：http://hz.wangshuangyany.cn/gtecfawsjw.html

#define X_H
来源：http://hz.shanyushiyangkeji.top/gtmmcubwqt.html

#endif
来源：http://hz.yj20258.top/gtvcvkywbs.html

[S31] C++：Hello World
来源：http://hz.gzhubu.top/gtjpjbfvsd.html

#include <iostream>
来源：http://hz.yangfankeji.com/gteohswclw.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.316326.xyz/gtnxzkbyzm.html

[S32] C++：字符串
来源：http://hz.meibo888.top/gtuceomhuj.html

std::string s = "hi";  s += "!";
来源：http://hz.tian-w.cn/gtwxxcollr.html

[S33] C++：vector 增删
来源：http://hz.jinqigfzy.top/gtaofvbapx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.haohaochexian.top/gtvgdujryc.html

[S34] C++：遍历 vector
来源：http://hz.havefunace.top/gtylesprfd.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jinyuanbaomall.cn/gtzqgqdyfy.html

[S35] C++：map
来源：http://hz.chenlongwang.top/gtwhzctdiq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shanyushiyangtech.top/gtekldgwje.html

[S36] C++：unordered_map
来源：http://hz.0kj1m.cn/gtxgvjlekh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.smart0.xyz/gtfxsftgyz.html

[S37] C++：set
来源：http://hz.guowangkeji.top/gtlczwewlt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.shzxlz.cn/gtpvosmwbh.html

[S38] C++：排序
来源：http://hz.andypj.xyz/gtrpecitul.html

std::sort(v.begin(), v.end());
来源：http://hz.ppjwa.cn/gtagcrspeu.html

[S39] C++：自定义比较器排序
来源：http://hz.jyoumei.cn/gtfeivrkhp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.aizwys.cn/gttrpdqgsw.html

[S40] C++：查找元素
来源：http://hz.zhengqikj.top/gtvlosvrix.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.316326.xyz/gtrtslbgxh.html

[S41] C++：类与构造函数
来源：http://hz.jinyuanbaomall.cn/gtchzseord.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jiagoushi.top/gttdggboyd.html

[S42] C++：继承与虚函数
来源：http://hz.pycfn.com/gtkprwqurm.html

class B : public Base { public: void f() override {} };
来源：http://hz.sysykeji.top/gtvswsgsbj.html

[S43] C++：智能指针
来源：http://hz.nwbrower.top/gtfxikbxgo.html

auto p = std::make_unique<int>(5);
来源：http://hz.jqgfzy.top/gtdajlxwrm.html

[S44] C++：引用传参
来源：http://hz.dashuyun.cn/gtikbhjpbv.html

void inc(int &x) { ++x; }
来源：http://hz.52xcode.cn/gthwrlzgmi.html

[S45] C++：lambda
来源：http://hz.zhoulong.xyz/gtzybjauvg.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xinyue.icu/gtnwkjuavg.html

[S46] C++：函数模板
来源：http://hz.yangfankeji.com/gtxdgsnmei.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shanyushiyangkeji.top/gtuogvuwgf.html

[S47] C++：结构化绑定遍历
来源：http://hz.cqqwz.cn/gtnqccjbfb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shanyushiyangtech.top/gtcfrkcdao.html

[S48] C++：逐行读文件
来源：http://hz.yvedp.cn/gtnblaeppt.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ydjk.org.cn/gtffqeibbp.html

while (std::getline(in, line)) { }
来源：http://hz.zhiwuduotai.top/gtnytbegmj.html

[S49] C++：写文件
来源：http://hz.jiagoushi.top/gtxeydhkek.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.vqdsnc.cn/gtjmmygkwp.html

[S50] C++：格式化数字
来源：http://hz.sweek.top/gtpxhpfxpq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.tianlin.xyz/gtvjfsicbi.html

[S51] C++：显式类型转换
来源：http://hz.snrcjt.cn/gttdvumjab.html

static_cast<double>(a) / b
来源：http://hz.zhaomingkeji.xyz/gtuqagzjvk.html

[S52] C++：const 与 noexcept
来源：http://hz.shanyushiyangtech.top/gtglwivqmq.html


<!-- 参考信息 -->