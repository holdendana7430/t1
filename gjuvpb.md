代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.0kj1m.cn/gtnrekwoha.html

[Q75] 日期格式化
来源：http://hz.zhongyouzk.top/gtccygrqin.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ywan-chungtsiang.top/gtvyccsoow.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yvedp.cn/gtdsobhlxt.html

[Q76] 按天统计
来源：http://hz.ydjk.org.cn/gtccwmadfm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jlsjyb.cn/gtgoctrggk.html

[Q77] 时间加减
来源：http://hz.jinyuanbaomall.cn/gtwrbapgrk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.redwolf501.top/gttutqrexs.html

[Q78] 当前时间
来源：http://hz.wangshuangyany.cn/gtyxazuytm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.316326.xyz/gtczwtqcbk.html

[Q79] 字符串拼接
来源：http://hz.gaohongyu789.top/gthtmudteo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.gzhubu.top/gtltthlhpq.html

[Q80] 字符串截取
来源：http://hz.sxryk.cn/gtcocwssek.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.wangshuangyany.cn/gtuqudotgb.html

[Q81] 字符串替换
来源：http://hz.gzhubu.top/gtozdzfwtc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.kuanghao11.cn/gtywwmbnpa.html

[Q82] 字符长度与字节长度
来源：http://hz.quarkkingdee.top/gthwoosiud.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hnqzz.top/gtdylchxpo.html

[Q83] 大小写转换
来源：http://hz.andypj.xyz/gtplxbderb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.cheryme.top/gtffixocaq.html

[Q84] 去除首尾空格
来源：http://hz.zhaomingkeji.xyz/gtqnbqkyet.html

SELECT TRIM(name) FROM users;
来源：http://hz.yj20258.top/gtsgledpng.html

[Q85] 数值取整
来源：http://hz.gogol.net.cn/gtfqcekmwx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ywan-chungtsiang.top/gtbavmhyqt.html

[Q86] 读取 JSON 字段
来源：http://hz.ydzc1.top/gtsfbjhekt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.kuanghao11.cn/gtrevhnbxg.html

[Q87] JSON 字段做条件
来源：http://hz.gzhubu.top/gtobsiquvb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hywenlv.cn/gtapsktjdl.html

[Q88] 行转列（条件聚合）
来源：http://hz.cqqwz.cn/gtsiehuddb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhijiandao.cn/gtseyapuat.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xuanzx.com/gtudykknwp.html

[Q89] 判断表是否存在
来源：http://hz.fzhhl.top/gtqjmcyqmf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.cucudq.cn/gtbbvpcxhq.html

[Q90] 生成序号列
来源：http://hz.hywenlv.cn/gtcikhtgno.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ivvv.top/gtwwfszoyr.html

================================================================================
来源：http://hz.9152youxi.cn/gtmcadqmwv.html

R. Bash 专题
来源：http://hz.haohaochexian.top/gttusxxmns.html

================================================================================
来源：http://hz.jinqigfzy.top/gtntwfebww.html

[R01] shebang 与严格模式
来源：http://hz.jyoumei.cn/gtvxzadeqg.html

#!/usr/bin/env bash
来源：http://hz.andypj.xyz/gtsyudifow.html

set -euo pipefail
来源：http://hz.pengpengdd.cyou/gtlwhgdrak.html

[R02] 变量赋值与使用
来源：http://hz.hfpthk.cn/gteidoektu.html

name="Tom"; echo "$name"
来源：http://hz.jiagoushi.top/gtbpzcawoo.html

[R03] 只读变量
来源：http://hz.c1oappe.top/gtmjwefiyg.html

readonly PI=3.14
来源：http://hz.gaohongyu789.top/gtihhycpns.html

[R04] 位置参数
来源：http://hz.ydjk.org.cn/gtpadrlsak.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.shuidangran.top/gtkcxrvoat.html

[R05] 参数默认值
来源：http://hz.sufxvd.cn/gtuikdcqhz.html

name="${1:-default}"
来源：http://hz.zhiwuduotai.top/gtseicyfrz.html

[R06] 判断命令是否存在
来源：http://hz.redwolf501.top/gtftbuhiqi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.birdmap.top/gtbisozcpj.html

[R07] if 判断文件
来源：http://hz.sxryk.cn/gttwmaiuan.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.c1oappe.top/gtznirpvoj.html

[R08] 数值比较
来源：http://hz.hysaishi.cn/gtkmnjwuiy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zycfv.cn/gtfmcdlefg.html

[R09] 字符串比较
来源：http://hz.gaohongyu789.top/gtinuulwnf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.tianlin.xyz/gtokwfcizb.html

[R10] 正则匹配
来源：http://hz.xziqi.cn/gtzsnwgrpo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yvedp.cn/gtxvocergz.html

[R11] case 多分支
来源：http://hz.sxryk.cn/gtosbvryfh.html

case "$1" in
来源：http://hz.hongshengwenyu.top/gtcrzwckgx.html

start) echo "启动" ;;
来源：http://hz.smart0.xyz/gtfnfuyeoa.html

stop)  echo "停止" ;;
来源：http://hz.jinghuilouyu.cn/gtmoprkiku.html

*)     echo "未知命令" ;;
来源：http://hz.cdnleiting.top/gtotcqvutl.html

esac
来源：http://hz.daxiang520.top/gtanzxzfic.html

[R12] for 遍历文件
来源：http://hz.yongpay.top/gtubjceyrx.html

for f in *.txt; do echo "$f"; done
来源：http://hz.feifeiyinyue.top/gtmzkxsarj.html

[R13] for 计数循环
来源：http://hz.andypj.xyz/gtiajjuzii.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jinqigfzy.top/gtvonpsjte.html

[R14] C 风格 for
来源：http://hz.jinqigfzy.top/gtveqdddbm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cdnleiting.top/gtapwuxknb.html

[R15] while 逐行读文件
来源：http://hz.aizwys.cn/gtdktibucf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zdqjudy.top/gteahjotgf.html

[R16] until 等待条件
来源：http://hz.havefunace.top/gtcvelynqt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.xuetiantiany.cn/gtjbrkjeux.html

[R17] 数组定义与取值
来源：http://hz.bjfxy.top/gtooumaetq.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.aizwys.cn/gtdxtyzzwd.html

[R18] 遍历数组
来源：http://hz.kuanghao11.cn/gtmsqltktn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.nwbrower.top/gttumotiem.html

[R19] 数组长度
来源：http://hz.cheryme.top/gtvurbobmz.html

echo "${#arr[@]}"
来源：http://hz.hongshengwenyu.top/gtxsxonqio.html

[R20] 关联数组（字典）
来源：http://hz.cheryme.top/gtedjlbsjl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.dashuyun.cn/gtrxzadios.html

[R21] 字符串长度
来源：http://hz.ywan-chungtsiang.top/gtrgmrlgrx.html

echo "${#s}"
来源：http://hz.jqgfzy.top/gtlahagkbk.html

[R22] 截取子串
来源：http://hz.bjfxy.top/gtgflpjsog.html

echo "${s:0:5}"
来源：http://hz.zhixingplan.top/gtqryqkdik.html

[R23] 字符串替换
来源：http://hz.guannengcc.top/gtbbqrxcgi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.sxryk.cn/gthpgajsqo.html

[R24] 大小写转换
来源：http://hz.pengpengdd.cyou/gtzkhevppi.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.smart0.xyz/gtqrgabrao.html

[R25] 去后缀 / 去前缀
来源：http://hz.jqgufenzy.top/gtqgbojogw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.gzhubu.top/gtgkhmhrcb.html

[R26] 命令替换
来源：http://hz.wangdashe.top/gtribrcnlh.html

now=$(date +%F); echo "$now"
来源：http://hz.9152youxi.cn/gtcnokwklm.html

[R27] 算术展开
来源：http://hz.jyoumei.cn/gtwcghfepk.html

echo $((1 + 2 * 3))
来源：http://hz.zhengqikj.top/gtuypufgel.html

[R28] 浮点运算
来源：http://hz.hysaishi.cn/gtvikkimha.html

echo "scale=2; 10/3" | bc
来源：http://hz.xingfuxueyuan.xyz/gtxilqrfdl.html

[R29] 定义函数
来源：http://hz.xuanzx.com/gtuaciudnz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhoulong.xyz/gtmtyulczq.html

[R30] 函数返回状态码
来源：http://hz.ppjwa.cn/gtdkqbsbrq.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.vqdsnc.cn/gtmsvgpefo.html

[R31] 局部变量
来源：http://hz.jinghuilouyu.cn/gtskqcqeca.html

f() { local x=1; echo "$x"; }
来源：http://hz.c1oappe.top/gtasnzcycu.html

[R32] 参数个数校验
来源：http://hz.smart0.xyz/gtbkvaiuup.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yj20258.top/gttumhfygi.html

[R33] 捕获错误并提示行号
来源：http://hz.yuxming.cn/gtnwrjkhxh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zdqjudy.top/gtsaybbxrf.html

[R34] 退出时清理
来源：http://hz.c1oappe.top/gtpcqrlnaj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.smart0.xyz/gtoigvjvye.html

[R35] 后台执行并等待
来源：http://hz.chenzaomai.com/gtgrllrfnv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xziqi.cn/gttuqtksam.html

[R36] 并发执行多个任务
来源：http://hz.cdnleiting.top/gtwdwueleg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cqqwz.cn/gtfloqpzrl.html

[R37] 把输出赋给变量
来源：http://hz.andypj.xyz/gtllhesyyk.html

files=$(ls -1)
来源：http://hz.yuanzhike.top/gtyvzboatu.html

[R38] 管道串联
来源：http://hz.shanyushiyangtech.top/gtbyrlxrbw.html

cat a.txt | grep -i error | wc -l
来源：http://hz.sweek.top/gttnylzetl.html

[R39] 重定向标准输出与错误
来源：http://hz.sufxvd.cn/gtkjctuddx.html

cmd > out.log 2>&1
来源：http://hz.jianghu66.top/gtbnfzwkkg.html

[R40] 追加写日志
来源：http://hz.mhx1999.top/gtlznysbgl.html

echo "log" >> out.log
来源：http://hz.haohaochexian.top/gtrnoypilo.html

[R41] 丢弃输出
来源：http://hz.tian-w.cn/gtrziyfepp.html

cmd >/dev/null 2>&1
来源：http://hz.yangfankeji.com/gtlvpjfjaa.html

[R42] 输入重定向
来源：http://hz.ydjk.org.cn/gtxbcjkvas.html

wc -l < a.txt
来源：http://hz.xylfe.cn/gtvnnmudfv.html

[R43] 按名字查找文件
来源：http://hz.havefunace.top/gtchpgachc.html

find . -name "*.log" -type f
来源：http://hz.iojbl.cn/gtvnvjpyze.html

[R44] 按修改时间查找
来源：http://hz.jinghuilouyu.cn/gtcwkfeyim.html

find . -mtime -7 -type f
来源：http://hz.vqdsnc.cn/gtyyphajwz.html

[R45] 批量删除
来源：http://hz.smart0.xyz/gtuvryixjl.html

find . -name "*.tmp" -delete
来源：http://hz.xziqi.cn/gtooczacoa.html

[R46] 递归替换文件内容
来源：http://hz.yonumen.top/gtwbheqwvj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.wangdashe.top/gtnhnfwyrn.html

[R47] sed 单行替换
来源：http://hz.havefunace.top/gtreajjpwv.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ydjk.org.cn/gtolqfqhxc.html

[R48] awk 取指定列
来源：http://hz.vqdsnc.cn/gtiaojgthq.html

awk '{print $1, $3}' a.txt
来源：http://hz.chenlongwang.top/gtltaccadp.html

[R49] awk 带条件
来源：http://hz.guowangkeji.top/gtarafmnot.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.sxryk.cn/gtjuzsfkce.html

[R50] awk 求和
来源：http://hz.yangfankeji.com/gtpfkekilg.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.aibaodan.cn/gthgzajjmw.html

[R51] 排序去重取前几
来源：http://hz.ybcxt.top/gtwstxqoyj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shzxlz.cn/gtlfkyqrtk.html

[R52] 统计行数
来源：http://hz.ivvv.top/gtamjpysck.html

wc -l a.txt
来源：http://hz.yangfankeji.com/gtzbfymogh.html

[R53] 查看文件头与实时尾
来源：http://hz.shangyingyoupin.top/gtztvyqgqv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cheryme.top/gtiyujnetx.html

[R54] 比较两个文件
来源：http://hz.yj20258888.top/gtjucxdifq.html

diff a.txt b.txt
来源：http://hz.xingfuxueyuan.xyz/gtrxrvzzgb.html

[R55] 压缩与解压
来源：http://hz.chenlongwang.top/gtxnuwlfpq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ybcxt.top/gteoacxavj.html

[R56] 远程拷贝
来源：http://hz.shzxlz.cn/gtjuvgceij.html

scp file user@host:/path/
来源：http://hz.daxiang520.top/gtxnajqcke.html

[R57] 远程执行命令
来源：http://hz.sufxvd.cn/gtgrbzuydv.html

ssh user@host 'uptime'
来源：http://hz.jinyuanbaomall.cn/gtpnaajzdp.html

[R58] 下载文件
来源：http://hz.gotoacloud.top/gtrwwripkw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jyoumei.cn/gtaqhzrimb.html

[R59] 发 POST JSON
来源：http://hz.xuanzx.com/gterajoxab.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.pengpengdd.cyou/gtxvbbfada.html

[R60] 只看 HTTP 状态码
来源：http://hz.hywenlv.cn/gtzxymoeif.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ivvv.top/gtrrkcjyhr.html

[R61] 磁盘占用
来源：http://hz.aizwys.cn/gtopbsuqjh.html

df -h;  du -sh *
来源：http://hz.xinyue.icu/gtazrwqiwr.html

[R62] 找最占空间的文件
来源：http://hz.chenjidiqi.icu/gtnhppwhwd.html

du -ah . | sort -rh | head -10
来源：http://hz.9152youxi.cn/gtcvaiuzsy.html

[R63] 内存与进程
来源：http://hz.cheryme.top/gteyiqdwxn.html

free -h;  ps aux | grep nginx
来源：http://hz.ybcxt.top/gtsdvuupxv.html

[R64] 结束进程
来源：http://hz.fzhhl.top/gtjncdtwnf.html

kill -9 $(pgrep -f app.py)
来源：http://hz.smart0.xyz/gtjvriatet.html

[R65] 查看端口占用
来源：http://hz.jinyuanbaomall.cn/gttduaowaq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jyoumei.cn/gtepvjmdvm.html

[R66] 定时任务
来源：http://hz.redwolf501.top/gtozrsvsil.html

crontab -e;  crontab -l
来源：http://hz.daria6918.cn/gtsujolqnk.html

[R67] 生成随机十六进制串
来源：http://hz.xuanzx.com/gtweiotkyp.html

openssl rand -hex 16
来源：http://hz.jinyuanbaomall.cn/gtizzbkevi.html

[R68] 计算文件校验值
来源：http://hz.shanyushiyangtech.top/gtclnorwdo.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shanyushiyangtech.top/gtqehcfspr.html

[R69] 生成随机密码
来源：http://hz.nanxuanxn.top/gtpggsqrgt.html

head -c 16 /dev/urandom | base64
来源：http://hz.hnxiangtu.top/gtlemekohv.html

[R70] 时间戳与互转
来源：http://hz.shanyushiyangkeji.top/gtgqlmxhmi.html

date +%s;  date -d @1700000000
来源：http://hz.xziqi.cn/gtmrlkeokz.html

[R71] 日期格式化
来源：http://hz.redwolf501.top/gtfghczdfq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yj202588.top/gtaqjqpgdb.html

[R72] 等待端口就绪
来源：http://hz.cucudq.cn/gtdqkbeqpj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.daria6918.cn/gtycgwflcz.html

[R73] 分割大日志
来源：http://hz.feifeiyinyue.top/gteklnexfs.html

split -l 1000 big.log part_
来源：http://hz.cdnleiting.top/gtchihyaep.html

[R74] 批量重命名
来源：http://hz.ivvv.top/gtuvfvwtxn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.sysykeji.top/gtjgfxugzf.html

[R75] 导出环境变量
来源：http://hz.yj202588.top/gtesymakhc.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.bjfxy.top/gtwsiopozf.html

[R76] 使用临时文件
来源：http://hz.jinqigufen.top/gtuodrnmgp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jlsjyb.cn/gtyqrvukti.html

[R77] 读取用户输入
来源：http://hz.chenzaomai.com/gtcjrtnzuv.html

read -rp "请输入: " ans
来源：http://hz.dashuyun.cn/gtrcixqdtb.html

[R78] 交互式菜单
来源：http://hz.pycfn.com/gtsobkxvyj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jyoumei.cn/gtezxujubo.html

[R79] 解析命令行选项
来源：http://hz.pycfn.com/gtlqiatllh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hywenlv.cn/gtvuoxkgib.html

[R80] 查看脚本执行耗时
来源：http://hz.zhaomingkeji.xyz/gtkmhnkhut.html

time ./run.sh
来源：http://hz.zhengqikj.top/gtdwnddwrp.html

================================================================================
来源：http://hz.9152youxi.cn/gtlrlieguw.html

S. C / C++ 专题
来源：http://hz.zhengqikj.top/gtprbaweor.html

================================================================================
来源：http://hz.kuanghao11.cn/gtwrnujrfo.html

[S01] C：Hello World
来源：http://hz.jinghuilouyu.cn/gtnafjrzbl.html

#include <stdio.h>
来源：http://hz.xylfe.cn/gtzorkitbn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.guannengcc.top/gtfzmalzdj.html

[S02] C：变量与格式化输出
来源：http://hz.0kj1m.cn/gtyfeirote.html

int a = 10; printf("%d\n", a);
来源：http://hz.jinqigfzy.top/gtzsfkejvy.html

[S03] C：读入整数
来源：http://hz.shanyushiyangtech.top/gtjyocbivm.html

int x; scanf("%d", &x);
来源：http://hz.yongpay.top/gtreehltif.html

[S04] C：字符串复制
来源：http://hz.jqgufenzy.top/gtxsbegjhu.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xylfe.cn/gthqvlmewp.html

[S05] C：字符串长度
来源：http://hz.zhijiandao.cn/gtqgpcuvts.html

strlen(s)
来源：http://hz.ppjwa.cn/gtzqskexbd.html

[S06] C：字符串比较
来源：http://hz.redwolf501.top/gtgbivmada.html

strcmp(a, b) == 0
来源：http://hz.ehwqpu.com/gtvtquctbu.html

[S07] C：数组遍历求和
来源：http://hz.jinyuanbaomall.cn/gtzadxqjgp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.chenzaomai.com/gtcdgikebo.html

[S08] C：动态内存分配与释放
来源：http://hz.meibo888.top/gtukdqswty.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.sxryk.cn/gtxbumfuvs.html

[S09] C：结构体定义与初始化
来源：http://hz.dianchejie.cn/gthigrqmih.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.birdmap.top/gtacvnzsud.html

[S10] C：指针与解引用
来源：http://hz.nanxinkj.top/gtjmjicbuh.html

int *p = &a;  *p = 5;
来源：http://hz.meibo888.top/gtpwhwhyta.html

[S11] C：逐行读文件
来源：http://hz.sweek.top/gtdqjjxgjs.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.cdnleiting.top/gtcbkbgcez.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yangfankeji.com/gtjdtgskga.html

fclose(f);
来源：http://hz.ydzc1.top/gtoqmxfvhn.html

[S12] C：写文件
来源：http://hz.shanyushiyangtech.top/gtzcwkufow.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yanxiufei.cn/gttkjfayut.html

[S13] C：宏定义
来源：http://hz.jinghuilouyu.cn/gtsqqrrofs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jiagoushi.top/gtpasdhnwj.html

[S14] C：枚举
来源：http://hz.hysaishi.cn/gtovvlgzrk.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ivvv.top/gtkmanvxib.html

[S15] C：类型转换
来源：http://hz.yangfankeji.com/gtktlbuxwe.html

(double) a / b
来源：http://hz.bjfxy.top/gtvvgoeuzm.html

[S16] C：位操作置位
来源：http://hz.xuanzx.com/gtufnkftuz.html

x |= (1 << 3);
来源：http://hz.wangdashe.top/gttjqvdocm.html

[S17] C：安全拼接字符串
来源：http://hz.gotoacloud.top/gtrsitzomy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.birdmap.top/gtbgooxzvk.html

[S18] C：命令行参数
来源：http://hz.hnqzz.top/gtyiphotlk.html

int main(int argc, char **argv)
来源：http://hz.zhiwuduotai.top/gtdbxswpkk.html

[S19] C：快速排序
来源：http://hz.tianlin.xyz/gtwulgbgec.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hysaishi.cn/gtcdtrszem.html

[S20] C：二分查找
来源：http://hz.9152youxi.cn/gtghzkrbrs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yj202588.top/gtwmmctztz.html

[S21] C：字符类别判断
来源：http://hz.ivvv.top/gtsyqzemmp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ybcxt.top/gtimypgowe.html

[S22] C：字符串转数字
来源：http://hz.kuanghao11.cn/gtvcihikwq.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.fzhhl.top/gtzpmbahzw.html

[S23] C：随机数
来源：http://hz.pycfn.com/gtnjlyaglk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.wangshuangyany.cn/gtnevejnwk.html

[S24] C：获取本地时间
来源：http://hz.xylfe.cn/gtohhgwlwb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.gzhubu.top/gtheblgndv.html

[S25] C：内存拷贝
来源：http://hz.nanxuanxn.top/gtpczlkscl.html

memcpy(dst, src, n);
来源：http://hz.tianlin.xyz/gtvhetrwla.html

[S26] C：内存清零
来源：http://hz.ehwqpu.com/gtiyadsyef.html

memset(a, 0, sizeof a);
来源：http://hz.aibaodan.cn/gtpgxfhoas.html

[S27] C：定义常量
来源：http://hz.cheryme.top/gtioqvqelp.html

const double PI = 3.14159;
来源：http://hz.smart0.xyz/gtgntkrvyo.html

[S28] C：静态变量
来源：http://hz.xinyue.icu/gtfhchbbrf.html

static int counter = 0;
来源：http://hz.yvedp.cn/gtvhgdnadq.html

[S29] C：变参函数
来源：http://hz.ywan-chungtsiang.top/gtqyudhrgo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ydjk.org.cn/gtnlpwratt.html

[S30] C：头文件保护
来源：http://hz.jinyuanbaomall.cn/gtfzcgwhnu.html

#ifndef X_H
来源：http://hz.jianghu66.top/gtjjodwmoz.html

#define X_H
来源：http://hz.iojbl.cn/gtmyzqtgqb.html

#endif
来源：http://hz.jinqigufen.top/gtznphupsx.html

[S31] C++：Hello World
来源：http://hz.zhongyouzk.top/gtjuqcesni.html

#include <iostream>
来源：http://hz.hysaishi.cn/gtzdiwazye.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.sweek.top/gtxtfxeaml.html

[S32] C++：字符串
来源：http://hz.zhiwuduotai.top/gtbkjgpcon.html

std::string s = "hi";  s += "!";
来源：http://hz.xylfe.cn/gtidxfawpv.html

[S33] C++：vector 增删
来源：http://hz.sxryk.cn/gtqwjtaidl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.bjfxy.top/gtqtcfdtpq.html

[S34] C++：遍历 vector
来源：http://hz.yongpay.top/gtgpjupmtx.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yanxiufei.cn/gtgdpsbvjr.html

[S35] C++：map
来源：http://hz.andypj.xyz/gtbjiaibwu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.pycfn.com/gtpntulwik.html

[S36] C++：unordered_map
来源：http://hz.hysaishi.cn/gtjdogrmcd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.quarkkingdee.top/gtkcwvtlbw.html

[S37] C++：set
来源：http://hz.snrcjt.cn/gtunnuusea.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.vqdsnc.cn/gtkynabrxn.html

[S38] C++：排序
来源：http://hz.sufxvd.cn/gtaahivdwk.html

std::sort(v.begin(), v.end());
来源：http://hz.dashuyun.cn/gtuvrulvoj.html

[S39] C++：自定义比较器排序
来源：http://hz.haohaochexian.top/gtcnfotjuf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.tian-w.cn/gtnrannpiu.html

[S40] C++：查找元素
来源：http://hz.xinyue.icu/gtkpzqftte.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yuanzhike.top/gtkcowwebx.html

[S41] C++：类与构造函数
来源：http://hz.zhiwuduotai.top/gtvknbzacw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.quarkkingdee.top/gttrptmrzn.html

[S42] C++：继承与虚函数
来源：http://hz.zhongyouzk.top/gthodervca.html

class B : public Base { public: void f() override {} };
来源：http://hz.yj20258.top/gtqtppvsna.html

[S43] C++：智能指针
来源：http://hz.xziqi.cn/gtapkbujvl.html

auto p = std::make_unique<int>(5);
来源：http://hz.shuidangran.top/gtcjkxpwqr.html

[S44] C++：引用传参
来源：http://hz.sxryk.cn/gthvyjzdle.html

void inc(int &x) { ++x; }
来源：http://hz.shanyushiyangkeji.top/gtlkflehys.html


<!-- 参考信息 -->