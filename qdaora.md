代发 wailian999

ANALYZE TABLE users;
来源：http://hz.zhaomingkeji.xyz/gtekkrxytl.html

[Q71] 查看建表语句
来源：http://hz.chenlongwang.top/gtiamjbext.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xziqi.cn/gtdshnnpey.html

[Q72] 查看索引
来源：http://hz.ywan-chungtsiang.top/gttocpnaxe.html

SHOW INDEX FROM users;
来源：http://hz.hysaishi.cn/gtjxilgkem.html

[Q73] 查看表状态
来源：http://hz.feifeiyinyue.top/gtifpmilvo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.andypj.xyz/gtrbwstxww.html

[Q74] 强制使用索引
来源：http://hz.hnxiangtu.top/gtvfnocryr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zycfv.cn/gtgxmzcgwy.html

[Q75] 日期格式化
来源：http://hz.wangshuangyany.cn/gtehvksyyb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ydzc1.top/gtlceffgnv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.mhx1999.top/gtbmnxzzkc.html

[Q76] 按天统计
来源：http://hz.tianlin.xyz/gtpkcrrjcu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.cheryme.top/gtbmsfkngb.html

[Q77] 时间加减
来源：http://hz.9152youxi.cn/gtwhkzdgol.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.smart0.xyz/gtuurmhlhj.html

[Q78] 当前时间
来源：http://hz.jiagoushi.top/gtkpqhrcfs.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.daria6918.cn/gtnuyldnfu.html

[Q79] 字符串拼接
来源：http://hz.yj20258888.top/gtffitroti.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.fzhhl.top/gtwvvggzey.html

[Q80] 字符串截取
来源：http://hz.vqdsnc.cn/gtbodcfbeq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.gaohongyu789.top/gtyvsifvjr.html

[Q81] 字符串替换
来源：http://hz.tanke756.top/gtwpyacqdd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.feifeiyinyue.top/gtsalmphbl.html

[Q82] 字符长度与字节长度
来源：http://hz.yj20258888.top/gtrfdiintc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.fengsongda.top/gtvovkliwh.html

[Q83] 大小写转换
来源：http://hz.hysaishi.cn/gtmzajrfst.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jinghuilouyu.cn/gtulltfdhq.html

[Q84] 去除首尾空格
来源：http://hz.birdmap.top/gtqgjynqji.html

SELECT TRIM(name) FROM users;
来源：http://hz.vqdsnc.cn/gtjrzqyltz.html

[Q85] 数值取整
来源：http://hz.quarkkingdee.top/gtpbqhtgnq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.daxiang520.top/gtmmpmqibo.html

[Q86] 读取 JSON 字段
来源：http://hz.sysykeji.top/gtlahthoks.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.sxryk.cn/gtisiuyaxg.html

[Q87] JSON 字段做条件
来源：http://hz.daria6918.cn/gtskphvlcg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yj202588.top/gtlpqzykvt.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhoulong.xyz/gtrvcfvpsh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.gaohongyu789.top/gtfprluyiy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zycfv.cn/gteugfigyk.html

[Q89] 判断表是否存在
来源：http://hz.ydzc1.top/gtxauxkmdu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.sxryk.cn/gtaagdvcwk.html

[Q90] 生成序号列
来源：http://hz.9152youxi.cn/gtzmfgdwdm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yonumen.top/gtuvcirzxc.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtesjwfwtx.html

R. Bash 专题
来源：http://hz.9152youxi.cn/gtnsyfvsxf.html

================================================================================
来源：http://hz.0kj1m.cn/gtigtiwzgo.html

[R01] shebang 与严格模式
来源：http://hz.yangfankeji.com/gtjcndhitx.html

#!/usr/bin/env bash
来源：http://hz.nwbrower.top/gtmwhyuizg.html

set -euo pipefail
来源：http://hz.feifeiyinyue.top/gtheidxxtp.html

[R02] 变量赋值与使用
来源：http://hz.shuidangran.top/gtdulybcpg.html

name="Tom"; echo "$name"
来源：http://hz.jqgfzy.top/gtxfpuzlke.html

[R03] 只读变量
来源：http://hz.xylfe.cn/gtbeynuzxo.html

readonly PI=3.14
来源：http://hz.vqdsnc.cn/gtufqegrnp.html

[R04] 位置参数
来源：http://hz.cashguo.top/gtfdzjlpdj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cqqwz.cn/gtgyvksovp.html

[R05] 参数默认值
来源：http://hz.xylfe.cn/gtqmbwghgt.html

name="${1:-default}"
来源：http://hz.zhoulong.xyz/gtfnmpmevh.html

[R06] 判断命令是否存在
来源：http://hz.jlsjyb.cn/gtnsiesfev.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xinyue.icu/gtlnldasfg.html

[R07] if 判断文件
来源：http://hz.jqgufenzy.top/gtojzcxccq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.meibo888.top/gtcsaukdfn.html

[R08] 数值比较
来源：http://hz.nwbrower.top/gtrrosfmvc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.smart0.xyz/gtakotddmn.html

[R09] 字符串比较
来源：http://hz.jqgufenzy.top/gtdkpzswuq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yuanzhike.top/gtgphpagmi.html

[R10] 正则匹配
来源：http://hz.shangyingyoupin.top/gtttmcdpgn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.svipenyu.cn/gtrmlhjcnn.html

[R11] case 多分支
来源：http://hz.shangyingyoupin.top/gtothhitvx.html

case "$1" in
来源：http://hz.wangshuangyany.cn/gtauycffjw.html

start) echo "启动" ;;
来源：http://hz.mhx1999.top/gtkmjgemqx.html

stop)  echo "停止" ;;
来源：http://hz.hfpthk.cn/gthxgukyeo.html

*)     echo "未知命令" ;;
来源：http://hz.snrcjt.cn/gtvfqzyjja.html

esac
来源：http://hz.yj20258.top/gthjyrhdbn.html

[R12] for 遍历文件
来源：http://hz.hongshengwenyu.top/gtbashfytj.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jianghu66.top/gtdqtdkalc.html

[R13] for 计数循环
来源：http://hz.jinqigufen.top/gtqnpnqvtx.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.0kj1m.cn/gtdrmginqa.html

[R14] C 风格 for
来源：http://hz.nwbrower.top/gtvwzhdvhd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jyoumei.cn/gtkctqsqse.html

[R15] while 逐行读文件
来源：http://hz.wangdashe.top/gtmwmzanjx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.aibaodan.cn/gtzrofkzps.html

[R16] until 等待条件
来源：http://hz.hfpthk.cn/gtxgdqkrwq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.svipenyu.cn/gtxbdpdgqu.html

[R17] 数组定义与取值
来源：http://hz.tian-w.cn/gteujvjqzq.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.iojbl.cn/gtsqlsnyzq.html

[R18] 遍历数组
来源：http://hz.jinyuanbaomall.cn/gtttcusary.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jlsjyb.cn/gtifwtekla.html

[R19] 数组长度
来源：http://hz.jqgufenzy.top/gtpmxpefjr.html

echo "${#arr[@]}"
来源：http://hz.ybcxt.top/gtovvizffc.html

[R20] 关联数组（字典）
来源：http://hz.9152youxi.cn/gtnurkwvpa.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jqgfzy.top/gtpwasbcyd.html

[R21] 字符串长度
来源：http://hz.c1oappe.top/gtospitkuq.html

echo "${#s}"
来源：http://hz.cdnleiting.top/gtwlklqyca.html

[R22] 截取子串
来源：http://hz.hywenlv.cn/gtktxmkavp.html

echo "${s:0:5}"
来源：http://hz.cheryme.top/gtldwihgxz.html

[R23] 字符串替换
来源：http://hz.ydzc1.top/gtpehuidgn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ivvv.top/gtszlhogzh.html

[R24] 大小写转换
来源：http://hz.zycfv.cn/gtvbckezhs.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.smart0.xyz/gtfpzngqhh.html

[R25] 去后缀 / 去前缀
来源：http://hz.hfpthk.cn/gtibmaohim.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xylfe.cn/gtfnrhtscq.html

[R26] 命令替换
来源：http://hz.yj20258.top/gtjxpudtgk.html

now=$(date +%F); echo "$now"
来源：http://hz.jinghuilouyu.cn/gtcxnhrddl.html

[R27] 算术展开
来源：http://hz.kuanghao11.cn/gtmjhwjepv.html

echo $((1 + 2 * 3))
来源：http://hz.ywan-chungtsiang.top/gtlyxbxruk.html

[R28] 浮点运算
来源：http://hz.jqgfzy.top/gtdolcblsv.html

echo "scale=2; 10/3" | bc
来源：http://hz.hfpthk.cn/gtrwyffzal.html

[R29] 定义函数
来源：http://hz.xuetiantiany.cn/gtapnlsttn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.gaohongyu789.top/gtoiwejxvs.html

[R30] 函数返回状态码
来源：http://hz.ydzc1.top/gtexkgvknx.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.9152youxi.cn/gtlnhtiyfh.html

[R31] 局部变量
来源：http://hz.xylfe.cn/gtlnkujaog.html

f() { local x=1; echo "$x"; }
来源：http://hz.0kj1m.cn/gtpdrllxyl.html

[R32] 参数个数校验
来源：http://hz.cheryme.top/gttfpysqrc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.chenzaomai.com/gtzhzsfseg.html

[R33] 捕获错误并提示行号
来源：http://hz.ydzc1.top/gttypmujvg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ydjk.org.cn/gtcbidubwc.html

[R34] 退出时清理
来源：http://hz.havefunace.top/gtvjtmzuxw.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.haohaochexian.top/gtjywxmbca.html

[R35] 后台执行并等待
来源：http://hz.yuxming.cn/gttdrqyubn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yj20258.top/gtcksinqnz.html

[R36] 并发执行多个任务
来源：http://hz.aibaodan.cn/gtnqdzznvu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yuanzhike.top/gtlutiumim.html

[R37] 把输出赋给变量
来源：http://hz.jqgufenzy.top/gtrrleaxsv.html

files=$(ls -1)
来源：http://hz.jqgufenzy.top/gtbxsgjykc.html

[R38] 管道串联
来源：http://hz.jiagoushi.top/gtbepsbdej.html

cat a.txt | grep -i error | wc -l
来源：http://hz.daxiang520.top/gtzjdhjknd.html

[R39] 重定向标准输出与错误
来源：http://hz.jyoumei.cn/gttlzsoepw.html

cmd > out.log 2>&1
来源：http://hz.zycfv.cn/gtkzvruejc.html

[R40] 追加写日志
来源：http://hz.ehwqpu.com/gtoqxoovru.html

echo "log" >> out.log
来源：http://hz.hnxiangtu.top/gtlfzspemf.html

[R41] 丢弃输出
来源：http://hz.vqdsnc.cn/gtxoibgfcp.html

cmd >/dev/null 2>&1
来源：http://hz.zhijiandao.cn/gtgjstnfqm.html

[R42] 输入重定向
来源：http://hz.fengsongda.top/gtgcjybcgb.html

wc -l < a.txt
来源：http://hz.cheryme.top/gtxxqzlsxn.html

[R43] 按名字查找文件
来源：http://hz.yj20258888.top/gtromvotnx.html

find . -name "*.log" -type f
来源：http://hz.jyoumei.cn/gtwotqmgrb.html

[R44] 按修改时间查找
来源：http://hz.tanke756.top/gttidsnjsj.html

find . -mtime -7 -type f
来源：http://hz.gotoacloud.top/gtyalwwxey.html

[R45] 批量删除
来源：http://hz.yonumen.top/gtbppydihw.html

find . -name "*.tmp" -delete
来源：http://hz.guowangkeji.top/gtcmzctiqc.html

[R46] 递归替换文件内容
来源：http://hz.zdqjudy.top/gtextamitb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ywan-chungtsiang.top/gtzpimcknw.html

[R47] sed 单行替换
来源：http://hz.andypj.xyz/gtefnugspn.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xylfe.cn/gtieeinsza.html

[R48] awk 取指定列
来源：http://hz.mhx1999.top/gtzkacytnk.html

awk '{print $1, $3}' a.txt
来源：http://hz.hysaishi.cn/gtridxnyen.html

[R49] awk 带条件
来源：http://hz.yvedp.cn/gtnsivbwqf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.cqqwz.cn/gtnoabeflg.html

[R50] awk 求和
来源：http://hz.shanyushiyangkeji.top/gtfumsxozy.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.shanyushiyangtech.top/gtslttuatx.html

[R51] 排序去重取前几
来源：http://hz.tianlin.xyz/gtzifkmwcr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shzxlz.cn/gtjxrgvjvw.html

[R52] 统计行数
来源：http://hz.hnqzz.top/gtgalulvmp.html

wc -l a.txt
来源：http://hz.xinyue.icu/gtmjldsjue.html

[R53] 查看文件头与实时尾
来源：http://hz.ydjk.org.cn/gtzyiiiwyb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hnqzz.top/gtivqdjbfu.html

[R54] 比较两个文件
来源：http://hz.tianlin.xyz/gtwirkqpab.html

diff a.txt b.txt
来源：http://hz.yvedp.cn/gtjriatenv.html

[R55] 压缩与解压
来源：http://hz.nanxuanxn.top/gtjsbuayle.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.cashguo.top/gtiatnolco.html

[R56] 远程拷贝
来源：http://hz.yongpay.top/gtfwyqkbnu.html

scp file user@host:/path/
来源：http://hz.cqqwz.cn/gtqwwkswkh.html

[R57] 远程执行命令
来源：http://hz.cheryme.top/gtlookzhny.html

ssh user@host 'uptime'
来源：http://hz.jinqigufen.top/gtkfoaapfc.html

[R58] 下载文件
来源：http://hz.snrcjt.cn/gtomdjwtno.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ybcxt.top/gtmslfnjlk.html

[R59] 发 POST JSON
来源：http://hz.xingfuxueyuan.xyz/gtjbriqblf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yuxming.cn/gtabwcayxf.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhongyouzk.top/gtjysneuii.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.wangshuangyany.cn/gtcfkdbdeq.html

[R61] 磁盘占用
来源：http://hz.cdnleiting.top/gtfzgfratw.html

df -h;  du -sh *
来源：http://hz.zhiwuduotai.top/gtthjgjwyo.html

[R62] 找最占空间的文件
来源：http://hz.shangyingyoupin.top/gtnszxstsg.html

du -ah . | sort -rh | head -10
来源：http://hz.yuanzhike.top/gtyebmrpmd.html

[R63] 内存与进程
来源：http://hz.zdqjudy.top/gtiweeaqon.html

free -h;  ps aux | grep nginx
来源：http://hz.shanyushiyangkeji.top/gtbqhmfcit.html

[R64] 结束进程
来源：http://hz.jinghuilouyu.cn/gtdbzixryq.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zdqjudy.top/gtmgitykmw.html

[R65] 查看端口占用
来源：http://hz.guannengcc.top/gtuhelubat.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.sxryk.cn/gtarmselph.html

[R66] 定时任务
来源：http://hz.xinyue.icu/gtlfycqjnr.html

crontab -e;  crontab -l
来源：http://hz.gotoacloud.top/gtdzqxhwru.html

[R67] 生成随机十六进制串
来源：http://hz.gotoacloud.top/gthqrpdznm.html

openssl rand -hex 16
来源：http://hz.shangyingyoupin.top/gtaywuwaak.html

[R68] 计算文件校验值
来源：http://hz.jlsjyb.cn/gtgrwtxrve.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xingfuxueyuan.xyz/gtyvunzkzy.html

[R69] 生成随机密码
来源：http://hz.haohaochexian.top/gtvdiwibcz.html

head -c 16 /dev/urandom | base64
来源：http://hz.hammf.cn/gtqwypyrqy.html

[R70] 时间戳与互转
来源：http://hz.cqqwz.cn/gtiodyzyny.html

date +%s;  date -d @1700000000
来源：http://hz.wangshuangyany.cn/gtnnrxelfb.html

[R71] 日期格式化
来源：http://hz.9152youxi.cn/gtxhqbbszu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yanxiufei.cn/gtzdqepmiy.html

[R72] 等待端口就绪
来源：http://hz.havefunace.top/gtpdgsyurj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.daxiang520.top/gtepjytutj.html

[R73] 分割大日志
来源：http://hz.nanxuanxn.top/gtymmyxccz.html

split -l 1000 big.log part_
来源：http://hz.0kj1m.cn/gtzheuhfpr.html

[R74] 批量重命名
来源：http://hz.jinghuilouyu.cn/gtelczsfdn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.cheryme.top/gtpxgznbaj.html

[R75] 导出环境变量
来源：http://hz.yuxming.cn/gtubxulcsx.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhongyouzk.top/gtxqmettwx.html

[R76] 使用临时文件
来源：http://hz.yonumen.top/gtkvilpnpj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.cdnleiting.top/gtmncgjeeh.html

[R77] 读取用户输入
来源：http://hz.yj20258888.top/gtoxagtpyb.html

read -rp "请输入: " ans
来源：http://hz.xziqi.cn/gtzcoawfpo.html

[R78] 交互式菜单
来源：http://hz.sysykeji.top/gtkboyagbj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhoulong.xyz/gtlthvljwn.html

[R79] 解析命令行选项
来源：http://hz.gogol.net.cn/gtkyybzlyd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hfpthk.cn/gtreommisi.html

[R80] 查看脚本执行耗时
来源：http://hz.yvedp.cn/gtfwtznxak.html

time ./run.sh
来源：http://hz.jinghuilouyu.cn/gtycvpakzd.html

================================================================================
来源：http://hz.shzxlz.cn/gtkqxjrdui.html

S. C / C++ 专题
来源：http://hz.ppjwa.cn/gtszflqwgj.html

================================================================================
来源：http://hz.xuanzx.com/gtbeszqvtz.html

[S01] C：Hello World
来源：http://hz.cheryme.top/gttqvrjxxz.html

#include <stdio.h>
来源：http://hz.xuanzx.com/gthrifvfri.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hongshengwenyu.top/gtvrgdwiwf.html

[S02] C：变量与格式化输出
来源：http://hz.ivvv.top/gtnfksjjtk.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhixingplan.top/gthshzgkwm.html

[S03] C：读入整数
来源：http://hz.yj20258.top/gtwknfuets.html

int x; scanf("%d", &x);
来源：http://hz.shanyushiyangkeji.top/gttivlvhvp.html

[S04] C：字符串复制
来源：http://hz.zhixingplan.top/gtavyjxypy.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yangfankeji.com/gtuftkmngj.html

[S05] C：字符串长度
来源：http://hz.feifeiyinyue.top/gtxpahmwvr.html

strlen(s)
来源：http://hz.xingfuxueyuan.xyz/gtsneqpzvw.html

[S06] C：字符串比较
来源：http://hz.meibo888.top/gtjooezhmq.html

strcmp(a, b) == 0
来源：http://hz.xinyue.icu/gtwzaesfzj.html

[S07] C：数组遍历求和
来源：http://hz.guowangkeji.top/gthyxzatmk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.sufxvd.cn/gtclfiiksj.html

[S08] C：动态内存分配与释放
来源：http://hz.tian-w.cn/gtzinhvhfi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hongshengwenyu.top/gtxzridwhb.html

[S09] C：结构体定义与初始化
来源：http://hz.xuetiantiany.cn/gtohaujnat.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ydzc1.top/gtujstrzyy.html

[S10] C：指针与解引用
来源：http://hz.shanyushiyangtech.top/gtbcqectmq.html

int *p = &a;  *p = 5;
来源：http://hz.ydzc1.top/gtnrtmqerv.html

[S11] C：逐行读文件
来源：http://hz.nwbrower.top/gtcqziyagt.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.redwolf501.top/gtdytafmoz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.dianchejie.cn/gtwosayhws.html

fclose(f);
来源：http://hz.nanxinkj.top/gtkhyvsxcy.html

[S12] C：写文件
来源：http://hz.guannengcc.top/gtfzjwgjvl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.gzhubu.top/gtmqnasrcr.html

[S13] C：宏定义
来源：http://hz.fzhhl.top/gtwfoilmux.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.nwbrower.top/gtlnfhkpwp.html

[S14] C：枚举
来源：http://hz.feifeiyinyue.top/gtecotaafm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xingfuxueyuan.xyz/gtkfvpyroj.html

[S15] C：类型转换
来源：http://hz.pycfn.com/gtnpwznjnl.html

(double) a / b
来源：http://hz.zhixingplan.top/gtbpzrcoxn.html

[S16] C：位操作置位
来源：http://hz.smart0.xyz/gtapcabvck.html

x |= (1 << 3);
来源：http://hz.9152youxi.cn/gtdqnrlnyz.html

[S17] C：安全拼接字符串
来源：http://hz.aibaodan.cn/gtwwnltzgv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ydjk.org.cn/gttzillmag.html

[S18] C：命令行参数
来源：http://hz.aizwys.cn/gtjsusyldq.html

int main(int argc, char **argv)
来源：http://hz.ydjk.org.cn/gtuhrinfki.html

[S19] C：快速排序
来源：http://hz.jqgfzy.top/gtruehiwqq.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jqgufenzy.top/gtfwkxuuoj.html

[S20] C：二分查找
来源：http://hz.wangdashe.top/gtevqpeeob.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hywenlv.cn/gthgezlcgf.html

[S21] C：字符类别判断
来源：http://hz.316326.xyz/gtfzohghqr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.guannengcc.top/gtewxuawus.html

[S22] C：字符串转数字
来源：http://hz.havefunace.top/gtvuxfmarf.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ywan-chungtsiang.top/gtjjiakdyz.html

[S23] C：随机数
来源：http://hz.gaohongyu789.top/gtcbgwoxpy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jyoumei.cn/gtmemhuccm.html

[S24] C：获取本地时间
来源：http://hz.yangfankeji.com/gtcegdcbqh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xuanzx.com/gtwmlwfbkn.html

[S25] C：内存拷贝
来源：http://hz.sysykeji.top/gtojdpwmqp.html

memcpy(dst, src, n);
来源：http://hz.nanxuanxn.top/gtfyiirayf.html

[S26] C：内存清零
来源：http://hz.jinqigfzy.top/gtgszlgjsx.html

memset(a, 0, sizeof a);
来源：http://hz.yuxming.cn/gtftafjwqv.html

[S27] C：定义常量
来源：http://hz.jiagoushi.top/gtpzngrctl.html

const double PI = 3.14159;
来源：http://hz.c1oappe.top/gtvsjqqzpr.html

[S28] C：静态变量
来源：http://hz.0kj1m.cn/gtssbggxog.html

static int counter = 0;
来源：http://hz.jinghuilouyu.cn/gtofyhozgv.html

[S29] C：变参函数
来源：http://hz.shangyingyoupin.top/gtrbzmsimm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.kuanghao11.cn/gtawqmtxss.html

[S30] C：头文件保护
来源：http://hz.smart0.xyz/gttgfprkvs.html

#ifndef X_H
来源：http://hz.guowangkeji.top/gtskitxljr.html

#define X_H
来源：http://hz.tian-w.cn/gtpkxdorwa.html

#endif
来源：http://hz.shanyushiyangkeji.top/gtohcbchak.html

[S31] C++：Hello World
来源：http://hz.52xcode.cn/gtmhvppzxt.html

#include <iostream>
来源：http://hz.dianchejie.cn/gtzbhwaulh.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.wangdashe.top/gtuaunnppi.html

[S32] C++：字符串
来源：http://hz.yonumen.top/gtrixvgjfc.html

std::string s = "hi";  s += "!";
来源：http://hz.hywenlv.cn/gtdquxanlf.html

[S33] C++：vector 增删
来源：http://hz.yueranfly.top/gtrmsoautk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jyoumei.cn/gtiokskaoa.html

[S34] C++：遍历 vector
来源：http://hz.xinyue.icu/gtohvcnbcb.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.fzhhl.top/gteqdngxif.html

[S35] C++：map
来源：http://hz.yueranfly.top/gtghueolvo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ybcxt.top/gtgbhzkfbk.html

[S36] C++：unordered_map
来源：http://hz.zhixingplan.top/gtyfdcnysa.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj20258888.top/gtqgvnrkkm.html

[S37] C++：set
来源：http://hz.daria6918.cn/gthjxifvyg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jinyuanbaomall.cn/gtofxapvyv.html

[S38] C++：排序
来源：http://hz.9152youxi.cn/gtkelenbos.html

std::sort(v.begin(), v.end());
来源：http://hz.hywenlv.cn/gtmqdrvjdl.html

[S39] C++：自定义比较器排序
来源：http://hz.iojbl.cn/gthafcowpi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.snrcjt.cn/gtjsjmfgop.html

[S40] C++：查找元素
来源：http://hz.zhaomingkeji.xyz/gtgongesmt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.0kj1m.cn/gtdgrsaexy.html


<!-- 参考信息 -->