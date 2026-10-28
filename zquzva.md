代发 wailian999

SHOW INDEX FROM users;
来源：http://hz.jiagoushi.top/gtjpxmkupa.html

[Q73] 查看表状态
来源：http://hz.jqgufenzy.top/gtlchkdnjq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cucudq.cn/gttinuzzhi.html

[Q74] 强制使用索引
来源：http://hz.daxiang520.top/gtsghzzhse.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xuetiantiany.cn/gtwlnhnynx.html

[Q75] 日期格式化
来源：http://hz.chenjidiqi.icu/gtnwjuzpqr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.nanxuanxn.top/gtjgdwybta.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ppjwa.cn/gtypquxazy.html

[Q76] 按天统计
来源：http://hz.xziqi.cn/gtewiliwcr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.daxiang520.top/gtnmcdupys.html

[Q77] 时间加减
来源：http://hz.yuxming.cn/gtmpyktmcy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.cqqwz.cn/gtlsfiusqb.html

[Q78] 当前时间
来源：http://hz.zhiwuduotai.top/gtmpfvpcuc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.gaohongyu789.top/gtlaydwcat.html

[Q79] 字符串拼接
来源：http://hz.xinyue.icu/gtjduaukqn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.316326.xyz/gthrtjvtlt.html

[Q80] 字符串截取
来源：http://hz.sxryk.cn/gtbashqtcs.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.guowangkeji.top/gtijeckevr.html

[Q81] 字符串替换
来源：http://hz.tian-w.cn/gtoalkmmxe.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.feifeiyinyue.top/gtiindlafx.html

[Q82] 字符长度与字节长度
来源：http://hz.yangfankeji.com/gtwrgonxtv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.gogol.net.cn/gtwwyupcds.html

[Q83] 大小写转换
来源：http://hz.feifeiyinyue.top/gtjbrpopgj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xylfe.cn/gtbfaigvws.html

[Q84] 去除首尾空格
来源：http://hz.yangfankeji.com/gtmijppjib.html

SELECT TRIM(name) FROM users;
来源：http://hz.tanke756.top/gtsjodqedj.html

[Q85] 数值取整
来源：http://hz.zhaomingkeji.xyz/gtcnqwugsd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.chenzaomai.com/gtvslrpmye.html

[Q86] 读取 JSON 字段
来源：http://hz.aibaodan.cn/gtdodbdscb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.fengsongda.top/gtkhjvrcti.html

[Q87] JSON 字段做条件
来源：http://hz.ybcxt.top/gtnsrslpgs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.cdnleiting.top/gtdptxtnrk.html

[Q88] 行转列（条件聚合）
来源：http://hz.hfpthk.cn/gtlieyqvvg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.xinyue.icu/gtdftfeeii.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.nwbrower.top/gtqfxwyjvh.html

[Q89] 判断表是否存在
来源：http://hz.fengsongda.top/gthtruagof.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhijiandao.cn/gtnwcfoaya.html

[Q90] 生成序号列
来源：http://hz.birdmap.top/gtairgvedb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xuetiantiany.cn/gteoizyjdi.html

================================================================================
来源：http://hz.dianchejie.cn/gtrohdvcoz.html

R. Bash 专题
来源：http://hz.zhengqikj.top/gtgssijqtz.html

================================================================================
来源：http://hz.hywenlv.cn/gthlfebfor.html

[R01] shebang 与严格模式
来源：http://hz.jinqigfzy.top/gtthmvzych.html

#!/usr/bin/env bash
来源：http://hz.nwbrower.top/gtciaodjza.html

set -euo pipefail
来源：http://hz.sysykeji.top/gtdtlzwvfs.html

[R02] 变量赋值与使用
来源：http://hz.sysykeji.top/gtbtoneujt.html

name="Tom"; echo "$name"
来源：http://hz.hfpthk.cn/gtqqtlezno.html

[R03] 只读变量
来源：http://hz.ivvv.top/gtaehplelh.html

readonly PI=3.14
来源：http://hz.dashuyun.cn/gtshjyaucs.html

[R04] 位置参数
来源：http://hz.tianlin.xyz/gtmebzwadn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.52xcode.cn/gtpgsspizx.html

[R05] 参数默认值
来源：http://hz.havefunace.top/gtzlqguunb.html

name="${1:-default}"
来源：http://hz.jianghu66.top/gtoaegnsmk.html

[R06] 判断命令是否存在
来源：http://hz.smart0.xyz/gtdnkepfyo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ybcxt.top/gtnvtnwyic.html

[R07] if 判断文件
来源：http://hz.hnqzz.top/gtdwdotiyr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yvedp.cn/gtoxsoxpqv.html

[R08] 数值比较
来源：http://hz.316326.xyz/gtwrlelhil.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zycfv.cn/gtyhkutaqp.html

[R09] 字符串比较
来源：http://hz.hysaishi.cn/gtjcoupdsc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.aibaodan.cn/gtemtwxvpg.html

[R10] 正则匹配
来源：http://hz.zhijiandao.cn/gtaomyrzec.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ybcxt.top/gtsbyqllds.html

[R11] case 多分支
来源：http://hz.yueranfly.top/gtlkwaunjl.html

case "$1" in
来源：http://hz.yvedp.cn/gthsbnazwv.html

start) echo "启动" ;;
来源：http://hz.gzhubu.top/gtgaeywlnv.html

stop)  echo "停止" ;;
来源：http://hz.tianlin.xyz/gtcezjlmvh.html

*)     echo "未知命令" ;;
来源：http://hz.zhoulong.xyz/gtozsybyyn.html

esac
来源：http://hz.gogol.net.cn/gtufixvjaz.html

[R12] for 遍历文件
来源：http://hz.haohaochexian.top/gtqytushsl.html

for f in *.txt; do echo "$f"; done
来源：http://hz.aizwys.cn/gtkikvoesr.html

[R13] for 计数循环
来源：http://hz.zycfv.cn/gtqvtawykw.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ywan-chungtsiang.top/gtvtzhwrlv.html

[R14] C 风格 for
来源：http://hz.jinqigufen.top/gtadrtpzaz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yanxiufei.cn/gtfqbsabhx.html

[R15] while 逐行读文件
来源：http://hz.gaohongyu789.top/gtomlqfvsp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.cheryme.top/gtczvieowh.html

[R16] until 等待条件
来源：http://hz.shanyushiyangkeji.top/gtkvmoqmrj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.cheryme.top/gtymydvfgz.html

[R17] 数组定义与取值
来源：http://hz.chenzaomai.com/gtgndhhoht.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.kuanghao11.cn/gtfqeyptir.html

[R18] 遍历数组
来源：http://hz.andypj.xyz/gtmkrnbrsq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.kuanghao11.cn/gtugqgxven.html

[R19] 数组长度
来源：http://hz.guannengcc.top/gtmeehagke.html

echo "${#arr[@]}"
来源：http://hz.jqgufenzy.top/gtpimcjkuq.html

[R20] 关联数组（字典）
来源：http://hz.hywenlv.cn/gtcfoohvga.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xziqi.cn/gtwixuhfmz.html

[R21] 字符串长度
来源：http://hz.xylfe.cn/gtzzmkyfxq.html

echo "${#s}"
来源：http://hz.yj20258888.top/gttmxluttd.html

[R22] 截取子串
来源：http://hz.zhongyouzk.top/gtgsgvshyk.html

echo "${s:0:5}"
来源：http://hz.daxiang520.top/gtbeovzjeo.html

[R23] 字符串替换
来源：http://hz.chenzaomai.com/gthgkmrkvl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shanyushiyangkeji.top/gtckzmvepp.html

[R24] 大小写转换
来源：http://hz.bjfxy.top/gtfdpujvhf.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.quarkkingdee.top/gtodnefllm.html

[R25] 去后缀 / 去前缀
来源：http://hz.chenjidiqi.icu/gtsykrumhr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.guannengcc.top/gttxecugfc.html

[R26] 命令替换
来源：http://hz.mhx1999.top/gtolknqfww.html

now=$(date +%F); echo "$now"
来源：http://hz.vqdsnc.cn/gtxcvzxspz.html

[R27] 算术展开
来源：http://hz.zhijiandao.cn/gttiofuonh.html

echo $((1 + 2 * 3))
来源：http://hz.chenlongwang.top/gtwvvvviwu.html

[R28] 浮点运算
来源：http://hz.fzhhl.top/gtasjbupgc.html

echo "scale=2; 10/3" | bc
来源：http://hz.ehwqpu.com/gtuatpgvhy.html

[R29] 定义函数
来源：http://hz.jinyuanbaomall.cn/gtbrehotct.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hysaishi.cn/gtdjzwpzkn.html

[R30] 函数返回状态码
来源：http://hz.ywan-chungtsiang.top/gtbwegrzqf.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.guannengcc.top/gttxgbpzbm.html

[R31] 局部变量
来源：http://hz.cucudq.cn/gthjsntarr.html

f() { local x=1; echo "$x"; }
来源：http://hz.yongpay.top/gttlkdoefh.html

[R32] 参数个数校验
来源：http://hz.jiagoushi.top/gtemxbbeyr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.feifeiyinyue.top/gtladmshum.html

[R33] 捕获错误并提示行号
来源：http://hz.52xcode.cn/gtftlylhwc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.nanxuanxn.top/gtzndyxlmh.html

[R34] 退出时清理
来源：http://hz.pycfn.com/gtsybjorbj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.snrcjt.cn/gtpfunzopy.html

[R35] 后台执行并等待
来源：http://hz.daxiang520.top/gttegryzld.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xuanzx.com/gtguhfktsr.html

[R36] 并发执行多个任务
来源：http://hz.xylfe.cn/gtwwrzcgta.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hammf.cn/gtyawcqler.html

[R37] 把输出赋给变量
来源：http://hz.xziqi.cn/gtgzblpvex.html

files=$(ls -1)
来源：http://hz.xinyue.icu/gtfzwovglh.html

[R38] 管道串联
来源：http://hz.ivvv.top/gtmbpqosqa.html

cat a.txt | grep -i error | wc -l
来源：http://hz.c1oappe.top/gtwvovuzwz.html

[R39] 重定向标准输出与错误
来源：http://hz.nanxinkj.top/gttbpvpgqq.html

cmd > out.log 2>&1
来源：http://hz.dashuyun.cn/gtwlzaowtc.html

[R40] 追加写日志
来源：http://hz.haohaochexian.top/gtvplkqxdh.html

echo "log" >> out.log
来源：http://hz.hywenlv.cn/gtbaiebjie.html

[R41] 丢弃输出
来源：http://hz.zhixingplan.top/gtxjrwlkew.html

cmd >/dev/null 2>&1
来源：http://hz.mhx1999.top/gtephkruju.html

[R42] 输入重定向
来源：http://hz.xylfe.cn/gtcslkqwdx.html

wc -l < a.txt
来源：http://hz.yuanzhike.top/gtbytpidkr.html

[R43] 按名字查找文件
来源：http://hz.tian-w.cn/gturaqsuxc.html

find . -name "*.log" -type f
来源：http://hz.snrcjt.cn/gtuujqfqkh.html

[R44] 按修改时间查找
来源：http://hz.tianlin.xyz/gtpgxytkoz.html

find . -mtime -7 -type f
来源：http://hz.jinghuilouyu.cn/gtkmylfupc.html

[R45] 批量删除
来源：http://hz.daxiang520.top/gtdmaubxmx.html

find . -name "*.tmp" -delete
来源：http://hz.xziqi.cn/gtajxebecp.html

[R46] 递归替换文件内容
来源：http://hz.feifeiyinyue.top/gtodveqxpn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.daria6918.cn/gtkxoulkmw.html

[R47] sed 单行替换
来源：http://hz.hnqzz.top/gthnugebhu.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.redwolf501.top/gtphwojjpe.html

[R48] awk 取指定列
来源：http://hz.hnqzz.top/gtwplxbpad.html

awk '{print $1, $3}' a.txt
来源：http://hz.316326.xyz/gtvcclnmzh.html

[R49] awk 带条件
来源：http://hz.xylfe.cn/gtieitgcop.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ydzc1.top/gtfkzueykn.html

[R50] awk 求和
来源：http://hz.cucudq.cn/gtqcxuydlu.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hysaishi.cn/gtidusxnib.html

[R51] 排序去重取前几
来源：http://hz.shzxlz.cn/gtgwtxqlpl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.hammf.cn/gtdxrcropb.html

[R52] 统计行数
来源：http://hz.sxryk.cn/gtvibjnldy.html

wc -l a.txt
来源：http://hz.yonumen.top/gtihsgjavf.html

[R53] 查看文件头与实时尾
来源：http://hz.ydjk.org.cn/gtdymrushl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhoulong.xyz/gtyffcghbn.html

[R54] 比较两个文件
来源：http://hz.xingfuxueyuan.xyz/gtdubmyjro.html

diff a.txt b.txt
来源：http://hz.gzhubu.top/gtrtxulaup.html

[R55] 压缩与解压
来源：http://hz.shanyushiyangkeji.top/gtykowslal.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhiwuduotai.top/gtljqcxqed.html

[R56] 远程拷贝
来源：http://hz.quarkkingdee.top/gtgsntkfka.html

scp file user@host:/path/
来源：http://hz.daria6918.cn/gtdxhvwlxt.html

[R57] 远程执行命令
来源：http://hz.yj202588.top/gtigjzlydh.html

ssh user@host 'uptime'
来源：http://hz.ehwqpu.com/gtyyouvnql.html

[R58] 下载文件
来源：http://hz.nwbrower.top/gtnqkwwiun.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jqgufenzy.top/gtziykoijn.html

[R59] 发 POST JSON
来源：http://hz.zhaomingkeji.xyz/gtxhmwtceg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ivvv.top/gttegynofi.html

[R60] 只看 HTTP 状态码
来源：http://hz.jqgfzy.top/gttbbwamcp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ydzc1.top/gtclnywgcl.html

[R61] 磁盘占用
来源：http://hz.guannengcc.top/gthpaunddu.html

df -h;  du -sh *
来源：http://hz.cdnleiting.top/gtnvgcgzue.html

[R62] 找最占空间的文件
来源：http://hz.sysykeji.top/gtfbjrxkmk.html

du -ah . | sort -rh | head -10
来源：http://hz.nanxinkj.top/gtehruyuns.html

[R63] 内存与进程
来源：http://hz.jinyuanbaomall.cn/gtgdrdayjk.html

free -h;  ps aux | grep nginx
来源：http://hz.jqgufenzy.top/gtchkiayer.html

[R64] 结束进程
来源：http://hz.zhaomingkeji.xyz/gtwuhqgvgd.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ybcxt.top/gtwftewyas.html

[R65] 查看端口占用
来源：http://hz.zhijiandao.cn/gtvucxrbkk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.cheryme.top/gtzockxmtj.html

[R66] 定时任务
来源：http://hz.ydzc1.top/gtbqsjfndh.html

crontab -e;  crontab -l
来源：http://hz.9152youxi.cn/gtlatcbpza.html

[R67] 生成随机十六进制串
来源：http://hz.ehwqpu.com/gtnjhrreua.html

openssl rand -hex 16
来源：http://hz.yj202588.top/gtcnpncbre.html

[R68] 计算文件校验值
来源：http://hz.zhixingplan.top/gtjqjoacte.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hysaishi.cn/gtkzxmlujh.html

[R69] 生成随机密码
来源：http://hz.xuanzx.com/gtdnqxniqv.html

head -c 16 /dev/urandom | base64
来源：http://hz.haohaochexian.top/gthafjfpqd.html

[R70] 时间戳与互转
来源：http://hz.gzhubu.top/gtswdlwyhc.html

date +%s;  date -d @1700000000
来源：http://hz.kuanghao11.cn/gtwgdqcdru.html

[R71] 日期格式化
来源：http://hz.jinqigfzy.top/gtmmtwtgzn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yongpay.top/gtmhmzmfpj.html

[R72] 等待端口就绪
来源：http://hz.smart0.xyz/gtqmwyfnyb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ivvv.top/gtpisxbofw.html

[R73] 分割大日志
来源：http://hz.haohaochexian.top/gtxdrigfsk.html

split -l 1000 big.log part_
来源：http://hz.hfpthk.cn/gtrprnzswe.html

[R74] 批量重命名
来源：http://hz.yongpay.top/gtuzkbqayx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.9152youxi.cn/gthaoifluh.html

[R75] 导出环境变量
来源：http://hz.quarkkingdee.top/gtyamhzoar.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.havefunace.top/gtkknhkyrx.html

[R76] 使用临时文件
来源：http://hz.ywan-chungtsiang.top/gtgkwhzzth.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.tianlin.xyz/gttpwsegqb.html

[R77] 读取用户输入
来源：http://hz.ehwqpu.com/gtrjysmskd.html

read -rp "请输入: " ans
来源：http://hz.daria6918.cn/gtsdnjhwgr.html

[R78] 交互式菜单
来源：http://hz.xingfuxueyuan.xyz/gtarhixwck.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jinqigfzy.top/gtdhbtuoac.html

[R79] 解析命令行选项
来源：http://hz.zhongyouzk.top/gtncbjzsnn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ydjk.org.cn/gtkmcnhyys.html

[R80] 查看脚本执行耗时
来源：http://hz.hfpthk.cn/gtngrezojt.html

time ./run.sh
来源：http://hz.tianlin.xyz/gtohxngoji.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtcwkpgopn.html

S. C / C++ 专题
来源：http://hz.kuanghao11.cn/gtbkvmvqxo.html

================================================================================
来源：http://hz.ydjk.org.cn/gtasdyroag.html

[S01] C：Hello World
来源：http://hz.zhengqikj.top/gttmkzjeyx.html

#include <stdio.h>
来源：http://hz.hysaishi.cn/gtrgvomrfg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yanxiufei.cn/gtzohbistl.html

[S02] C：变量与格式化输出
来源：http://hz.svipenyu.cn/gtpqgvnubk.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhaomingkeji.xyz/gtwiiqicma.html

[S03] C：读入整数
来源：http://hz.zycfv.cn/gtjbwttkfx.html

int x; scanf("%d", &x);
来源：http://hz.pengpengdd.cyou/gtmmjzycak.html

[S04] C：字符串复制
来源：http://hz.nanxinkj.top/gtoklpngjp.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hnqzz.top/gtdpdhcgki.html

[S05] C：字符串长度
来源：http://hz.zdqjudy.top/gtvkfvudla.html

strlen(s)
来源：http://hz.xuanzx.com/gtunjgotwn.html

[S06] C：字符串比较
来源：http://hz.shzxlz.cn/gthcftoopa.html

strcmp(a, b) == 0
来源：http://hz.jqgufenzy.top/gtixlekkku.html

[S07] C：数组遍历求和
来源：http://hz.tanke756.top/gtljgurllw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.tanke756.top/gtvwnxgnnt.html

[S08] C：动态内存分配与释放
来源：http://hz.zhengqikj.top/gtwoxnzozo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xylfe.cn/gtgwytpdto.html

[S09] C：结构体定义与初始化
来源：http://hz.chenzaomai.com/gttxzqywvo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.shzxlz.cn/gtuluvqetp.html

[S10] C：指针与解引用
来源：http://hz.yueranfly.top/gtcllpwumb.html

int *p = &a;  *p = 5;
来源：http://hz.zhongyouzk.top/gtvhslqmbu.html

[S11] C：逐行读文件
来源：http://hz.yanxiufei.cn/gtgljkhxnt.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.nanxuanxn.top/gtylldiuou.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.xylfe.cn/gtrwzrasqo.html

fclose(f);
来源：http://hz.ehwqpu.com/gtmmcclxac.html

[S12] C：写文件
来源：http://hz.jiagoushi.top/gthiusglgw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.0kj1m.cn/gtqbnfekjq.html

[S13] C：宏定义
来源：http://hz.jqgufenzy.top/gtpqrfijrp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.sweek.top/gtpstkujsn.html

[S14] C：枚举
来源：http://hz.zhongyouzk.top/gthdjtchwd.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jinqigfzy.top/gtthgigdhy.html

[S15] C：类型转换
来源：http://hz.zhengqikj.top/gtpfomhudh.html

(double) a / b
来源：http://hz.svipenyu.cn/gtzuqmszjp.html

[S16] C：位操作置位
来源：http://hz.yuxming.cn/gtahrlfkqn.html

x |= (1 << 3);
来源：http://hz.yvedp.cn/gtxrpfmjol.html

[S17] C：安全拼接字符串
来源：http://hz.316326.xyz/gtygmajxoi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.sufxvd.cn/gtvvfgemrh.html

[S18] C：命令行参数
来源：http://hz.ywan-chungtsiang.top/gtfubifywv.html

int main(int argc, char **argv)
来源：http://hz.hnqzz.top/gtyksjeogm.html

[S19] C：快速排序
来源：http://hz.zdqjudy.top/gtjageikyq.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.haohaochexian.top/gtgupkjepa.html

[S20] C：二分查找
来源：http://hz.fzhhl.top/gtcazggeaa.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.tian-w.cn/gtgmjdutbo.html

[S21] C：字符类别判断
来源：http://hz.daxiang520.top/gtkutucyhf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.havefunace.top/gtooodvzhf.html

[S22] C：字符串转数字
来源：http://hz.daria6918.cn/gtvuocnplc.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.havefunace.top/gtbwznrgbh.html

[S23] C：随机数
来源：http://hz.hammf.cn/gtsccqkwst.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jqgufenzy.top/gttfwlcgax.html

[S24] C：获取本地时间
来源：http://hz.cucudq.cn/gttbhqmncl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jinyuanbaomall.cn/gtardaepkl.html

[S25] C：内存拷贝
来源：http://hz.sufxvd.cn/gtkofxhhwt.html

memcpy(dst, src, n);
来源：http://hz.zhijiandao.cn/gtyljtyxey.html

[S26] C：内存清零
来源：http://hz.feifeiyinyue.top/gttehikbyi.html

memset(a, 0, sizeof a);
来源：http://hz.fengsongda.top/gtekkacyvw.html

[S27] C：定义常量
来源：http://hz.aibaodan.cn/gtoogzmzxd.html

const double PI = 3.14159;
来源：http://hz.yvedp.cn/gtdaejspik.html

[S28] C：静态变量
来源：http://hz.gogol.net.cn/gtuajjqaek.html

static int counter = 0;
来源：http://hz.wangshuangyany.cn/gtwmmdijed.html

[S29] C：变参函数
来源：http://hz.jyoumei.cn/gtdiriwmbi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.sufxvd.cn/gtargytztn.html

[S30] C：头文件保护
来源：http://hz.shzxlz.cn/gterzrtbrj.html

#ifndef X_H
来源：http://hz.ywan-chungtsiang.top/gtwwkzxbxu.html

#define X_H
来源：http://hz.xuetiantiany.cn/gtlbgdfhlq.html

#endif
来源：http://hz.ywan-chungtsiang.top/gtvilmwfkp.html

[S31] C++：Hello World
来源：http://hz.xziqi.cn/gtxgwnugom.html

#include <iostream>
来源：http://hz.gaohongyu789.top/gtaqzupziq.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.chenzaomai.com/gtdynjtrki.html

[S32] C++：字符串
来源：http://hz.mhx1999.top/gtahqeacci.html

std::string s = "hi";  s += "!";
来源：http://hz.aibaodan.cn/gtajdphevp.html

[S33] C++：vector 增删
来源：http://hz.meibo888.top/gthjueeenu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.birdmap.top/gtzhmyjwdj.html

[S34] C++：遍历 vector
来源：http://hz.nanxinkj.top/gtpotnrlzh.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.fzhhl.top/gtehrbbicj.html

[S35] C++：map
来源：http://hz.aibaodan.cn/gtjlqtaepo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.bjfxy.top/gtlzllrtvf.html

[S36] C++：unordered_map
来源：http://hz.fzhhl.top/gtenvzdxbp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.9152youxi.cn/gtnsvsfkrw.html

[S37] C++：set
来源：http://hz.daxiang520.top/gttdhvspwe.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ybcxt.top/gtfnxictuc.html

[S38] C++：排序
来源：http://hz.zhengqikj.top/gtsgvedjjy.html

std::sort(v.begin(), v.end());
来源：http://hz.xylfe.cn/gtejyyvthv.html

[S39] C++：自定义比较器排序
来源：http://hz.xuetiantiany.cn/gtxaxpruie.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.mhx1999.top/gtchaoyjzc.html

[S40] C++：查找元素
来源：http://hz.cheryme.top/gtqqkbqlsb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.svipenyu.cn/gtwoiwxezo.html

[S41] C++：类与构造函数
来源：http://hz.nanxuanxn.top/gtcultegej.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.daria6918.cn/gtexfbxltm.html

[S42] C++：继承与虚函数
来源：http://hz.zycfv.cn/gtsoqbttnj.html

class B : public Base { public: void f() override {} };
来源：http://hz.jinghuilouyu.cn/gtmdtgducw.html


<!-- 参考信息 -->