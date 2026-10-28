代发 wailian999

ROLLBACK TO sp1;
来源：http://hz.zdqjudy.top/gtuvggwdhz.html

[Q69] 查看执行计划
来源：http://hz.pycfn.com/gtqqmdeovb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.cucudq.cn/gtaxaligrn.html

[Q70] 更新统计信息
来源：http://hz.xuanzx.com/gtkgolxwrg.html

ANALYZE TABLE users;
来源：http://hz.kuanghao11.cn/gtfslkacqn.html

[Q71] 查看建表语句
来源：http://hz.iojbl.cn/gtdrvudvxp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.tian-w.cn/gtqvdlivxw.html

[Q72] 查看索引
来源：http://hz.shuidangran.top/gtrjgvjear.html

SHOW INDEX FROM users;
来源：http://hz.hongshengwenyu.top/gtukbndrpe.html

[Q73] 查看表状态
来源：http://hz.tanke756.top/gtxxxhccqi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yangfankeji.com/gtqgkpldvh.html

[Q74] 强制使用索引
来源：http://hz.hysaishi.cn/gtiwcxqqbr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.guowangkeji.top/gtuvqmewlb.html

[Q75] 日期格式化
来源：http://hz.hywenlv.cn/gtydrojgjz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jlsjyb.cn/gtzzwduwwb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.gaohongyu789.top/gtixcgebsb.html

[Q76] 按天统计
来源：http://hz.yanxiufei.cn/gtdotifvbi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yanxiufei.cn/gtlufxtijf.html

[Q77] 时间加减
来源：http://hz.hfpthk.cn/gtvsiyhmbl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.9152youxi.cn/gtsycvmpbe.html

[Q78] 当前时间
来源：http://hz.guannengcc.top/gtosnrsdon.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.cashguo.top/gtoaqexmmr.html

[Q79] 字符串拼接
来源：http://hz.ywan-chungtsiang.top/gtgqpzzsno.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhiwuduotai.top/gtdcjoopxv.html

[Q80] 字符串截取
来源：http://hz.wangshuangyany.cn/gtvyhwygqm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.chenzaomai.com/gtzvpnbuel.html

[Q81] 字符串替换
来源：http://hz.hfpthk.cn/gtwdlyklbz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yonumen.top/gthlpeqrlr.html

[Q82] 字符长度与字节长度
来源：http://hz.wangdashe.top/gttvejgdrh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hysaishi.cn/gtiwarphrr.html

[Q83] 大小写转换
来源：http://hz.zhiwuduotai.top/gtzadhhyri.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhaomingkeji.xyz/gtrlddsxqs.html

[Q84] 去除首尾空格
来源：http://hz.birdmap.top/gthzbikgqm.html

SELECT TRIM(name) FROM users;
来源：http://hz.yanxiufei.cn/gtbqfljohi.html

[Q85] 数值取整
来源：http://hz.zdqjudy.top/gtpawcnmod.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.tianlin.xyz/gtxeceknaz.html

[Q86] 读取 JSON 字段
来源：http://hz.jinghuilouyu.cn/gttwlgpcfh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jinqigfzy.top/gtworhgtvx.html

[Q87] JSON 字段做条件
来源：http://hz.tanke756.top/gtdfbwedit.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jlsjyb.cn/gthqyughdy.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhaomingkeji.xyz/gtzebsykpv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.nanxuanxn.top/gtotggbuya.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xinyue.icu/gtlauxegte.html

[Q89] 判断表是否存在
来源：http://hz.havefunace.top/gtggnolcks.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.nanxinkj.top/gtqriviogg.html

[Q90] 生成序号列
来源：http://hz.yuxming.cn/gtlzluncjd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yuanzhike.top/gtkwaqrnbl.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtqzshchtj.html

R. Bash 专题
来源：http://hz.chenlongwang.top/gtblecdorq.html

================================================================================
来源：http://hz.hammf.cn/gtcxqcwfoz.html

[R01] shebang 与严格模式
来源：http://hz.kuanghao11.cn/gtgzrlwbkr.html

#!/usr/bin/env bash
来源：http://hz.ivvv.top/gtxoelfdii.html

set -euo pipefail
来源：http://hz.cheryme.top/gtyxxieyvo.html

[R02] 变量赋值与使用
来源：http://hz.sxryk.cn/gtyjgxbnns.html

name="Tom"; echo "$name"
来源：http://hz.jinyuanbaomall.cn/gtgcumpalb.html

[R03] 只读变量
来源：http://hz.tian-w.cn/gthsyidxem.html

readonly PI=3.14
来源：http://hz.hysaishi.cn/gthpnonerw.html

[R04] 位置参数
来源：http://hz.ydjk.org.cn/gtaleqpmqu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.aibaodan.cn/gtinrnefzh.html

[R05] 参数默认值
来源：http://hz.jyoumei.cn/gtuspcpjyy.html

name="${1:-default}"
来源：http://hz.hywenlv.cn/gtkpzfduon.html

[R06] 判断命令是否存在
来源：http://hz.svipenyu.cn/gtnsltrjme.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shangyingyoupin.top/gttriuxaqg.html

[R07] if 判断文件
来源：http://hz.cheryme.top/gtxermvqzk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.wangdashe.top/gtyzfndryn.html

[R08] 数值比较
来源：http://hz.tanke756.top/gtbqcuupkp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ybcxt.top/gthjtbjlkd.html

[R09] 字符串比较
来源：http://hz.jianghu66.top/gtndshuywp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.shuidangran.top/gtlgfghvvd.html

[R10] 正则匹配
来源：http://hz.ybcxt.top/gtpqjwhtpd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.nanxinkj.top/gtdqlkfiiz.html

[R11] case 多分支
来源：http://hz.chenlongwang.top/gtjkxmwpwz.html

case "$1" in
来源：http://hz.ywan-chungtsiang.top/gtvvhgxttr.html

start) echo "启动" ;;
来源：http://hz.quarkkingdee.top/gtrzwjipps.html

stop)  echo "停止" ;;
来源：http://hz.birdmap.top/gtsjeekhjm.html

*)     echo "未知命令" ;;
来源：http://hz.snrcjt.cn/gthkgpblts.html

esac
来源：http://hz.guannengcc.top/gtcpyelmdv.html

[R12] for 遍历文件
来源：http://hz.zhaomingkeji.xyz/gtuswpptom.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hfpthk.cn/gtshcsuojg.html

[R13] for 计数循环
来源：http://hz.zdqjudy.top/gtgtdfowkn.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.cucudq.cn/gtddvzewzb.html

[R14] C 风格 for
来源：http://hz.guannengcc.top/gtqzvywqpk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hnqzz.top/gtfgqyygmc.html

[R15] while 逐行读文件
来源：http://hz.gaohongyu789.top/gtfwfqkuav.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.aibaodan.cn/gtpdnnbblu.html

[R16] until 等待条件
来源：http://hz.birdmap.top/gtiwvmkval.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yvedp.cn/gttzfamreq.html

[R17] 数组定义与取值
来源：http://hz.aibaodan.cn/gtxwdpcvjn.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ehwqpu.com/gtdzsjvwmc.html

[R18] 遍历数组
来源：http://hz.tianlin.xyz/gtwoezgsrd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.meibo888.top/gtismyyllz.html

[R19] 数组长度
来源：http://hz.daria6918.cn/gtoyuaalbe.html

echo "${#arr[@]}"
来源：http://hz.pengpengdd.cyou/gtupisosih.html

[R20] 关联数组（字典）
来源：http://hz.yanxiufei.cn/gtjtzjkmra.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jinyuanbaomall.cn/gtvvxjxyhv.html

[R21] 字符串长度
来源：http://hz.quarkkingdee.top/gtuazhgjui.html

echo "${#s}"
来源：http://hz.jinqigufen.top/gtjthobtmv.html

[R22] 截取子串
来源：http://hz.gotoacloud.top/gtvuaasupc.html

echo "${s:0:5}"
来源：http://hz.jqgufenzy.top/gtdwelyriz.html

[R23] 字符串替换
来源：http://hz.316326.xyz/gtomcgltrm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.wangdashe.top/gtttduocrt.html

[R24] 大小写转换
来源：http://hz.jyoumei.cn/gtvnrykntv.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.shanyushiyangtech.top/gtfdgeluoa.html

[R25] 去后缀 / 去前缀
来源：http://hz.chenzaomai.com/gtyydthebn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.shuidangran.top/gtmqotvuek.html

[R26] 命令替换
来源：http://hz.ehwqpu.com/gtuvxqhnmq.html

now=$(date +%F); echo "$now"
来源：http://hz.yuxming.cn/gtvepaokgp.html

[R27] 算术展开
来源：http://hz.hnqzz.top/gtgtzjoosl.html

echo $((1 + 2 * 3))
来源：http://hz.fzhhl.top/gtchulodwo.html

[R28] 浮点运算
来源：http://hz.nanxinkj.top/gtvqdmaiar.html

echo "scale=2; 10/3" | bc
来源：http://hz.jqgfzy.top/gtczycewpx.html

[R29] 定义函数
来源：http://hz.dashuyun.cn/gtfrzzwaza.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zycfv.cn/gtmwnyrmee.html

[R30] 函数返回状态码
来源：http://hz.wangshuangyany.cn/gtnxpbfolq.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hnqzz.top/gtyssuperg.html

[R31] 局部变量
来源：http://hz.yangfankeji.com/gtrassqnbo.html

f() { local x=1; echo "$x"; }
来源：http://hz.jqgfzy.top/gtetlgbkkc.html

[R32] 参数个数校验
来源：http://hz.vqdsnc.cn/gtmcxudwjt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ivvv.top/gtncjjpzxd.html

[R33] 捕获错误并提示行号
来源：http://hz.svipenyu.cn/gtgevhfoug.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.daria6918.cn/gtywruhxvd.html

[R34] 退出时清理
来源：http://hz.guowangkeji.top/gtxzvxpati.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenjidiqi.icu/gtedywanmv.html

[R35] 后台执行并等待
来源：http://hz.316326.xyz/gtlagxszry.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.cheryme.top/gtcnehxecz.html

[R36] 并发执行多个任务
来源：http://hz.mhx1999.top/gtwdseowqa.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhengqikj.top/gtadkpnsku.html

[R37] 把输出赋给变量
来源：http://hz.yonumen.top/gtszjsmumb.html

files=$(ls -1)
来源：http://hz.jlsjyb.cn/gtnpryhrqi.html

[R38] 管道串联
来源：http://hz.tianlin.xyz/gtnwsiwhnx.html

cat a.txt | grep -i error | wc -l
来源：http://hz.haohaochexian.top/gtneclvagh.html

[R39] 重定向标准输出与错误
来源：http://hz.xingfuxueyuan.xyz/gtfftjbizp.html

cmd > out.log 2>&1
来源：http://hz.pengpengdd.cyou/gtwlxypfgp.html

[R40] 追加写日志
来源：http://hz.gogol.net.cn/gtbhjmmomd.html

echo "log" >> out.log
来源：http://hz.snrcjt.cn/gtxiwskukc.html

[R41] 丢弃输出
来源：http://hz.ehwqpu.com/gtxtgvshth.html

cmd >/dev/null 2>&1
来源：http://hz.cdnleiting.top/gttoxrderg.html

[R42] 输入重定向
来源：http://hz.xinyue.icu/gtiniviabu.html

wc -l < a.txt
来源：http://hz.pycfn.com/gtaytgiwnk.html

[R43] 按名字查找文件
来源：http://hz.zhongyouzk.top/gtgxdctkvv.html

find . -name "*.log" -type f
来源：http://hz.cqqwz.cn/gtefhtutvc.html

[R44] 按修改时间查找
来源：http://hz.chenzaomai.com/gtwtkkwdqm.html

find . -mtime -7 -type f
来源：http://hz.tanke756.top/gtlntzkevr.html

[R45] 批量删除
来源：http://hz.ppjwa.cn/gtadvvaziy.html

find . -name "*.tmp" -delete
来源：http://hz.cucudq.cn/gtjukkhsog.html

[R46] 递归替换文件内容
来源：http://hz.jiagoushi.top/gtverqbrwl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yuxming.cn/gtfrllhzql.html

[R47] sed 单行替换
来源：http://hz.hywenlv.cn/gtyaxaotan.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.cheryme.top/gtlqehffcq.html

[R48] awk 取指定列
来源：http://hz.havefunace.top/gtepnmfjcj.html

awk '{print $1, $3}' a.txt
来源：http://hz.pengpengdd.cyou/gtzsgkdksk.html

[R49] awk 带条件
来源：http://hz.tanke756.top/gtvjfyzywb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.nanxuanxn.top/gtvsyqigzq.html

[R50] awk 求和
来源：http://hz.guowangkeji.top/gtymzcsgug.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.cqqwz.cn/gtnibpczru.html

[R51] 排序去重取前几
来源：http://hz.chenzaomai.com/gtuwabveut.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.tian-w.cn/gtdqqqfepu.html

[R52] 统计行数
来源：http://hz.jqgufenzy.top/gthxilfjyj.html

wc -l a.txt
来源：http://hz.iojbl.cn/gtlisybiuv.html

[R53] 查看文件头与实时尾
来源：http://hz.chenlongwang.top/gtclgplnfb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xylfe.cn/gtxqebwrcj.html

[R54] 比较两个文件
来源：http://hz.yj20258888.top/gtqcajfhes.html

diff a.txt b.txt
来源：http://hz.gzhubu.top/gtrjnvxcmx.html

[R55] 压缩与解压
来源：http://hz.0kj1m.cn/gtdkaeircy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.0kj1m.cn/gtdejmpslw.html

[R56] 远程拷贝
来源：http://hz.pycfn.com/gtvyqmooao.html

scp file user@host:/path/
来源：http://hz.zhixingplan.top/gtyzqrwpyl.html

[R57] 远程执行命令
来源：http://hz.tanke756.top/gtogqpnjxh.html

ssh user@host 'uptime'
来源：http://hz.cucudq.cn/gtnxaxchou.html

[R58] 下载文件
来源：http://hz.sxryk.cn/gtvgioxkfq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.chenjidiqi.icu/gtbcoecxtu.html

[R59] 发 POST JSON
来源：http://hz.tanke756.top/gtrpezzcov.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinghuilouyu.cn/gtukpblwbf.html

[R60] 只看 HTTP 状态码
来源：http://hz.xinyue.icu/gtffbngced.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.sysykeji.top/gteyyuacwy.html

[R61] 磁盘占用
来源：http://hz.zdqjudy.top/gtycblwxpx.html

df -h;  du -sh *
来源：http://hz.chenjidiqi.icu/gtuiskwfak.html

[R62] 找最占空间的文件
来源：http://hz.pycfn.com/gtxkxhijrl.html

du -ah . | sort -rh | head -10
来源：http://hz.guannengcc.top/gtsjvzcorl.html

[R63] 内存与进程
来源：http://hz.mhx1999.top/gtmkrpqfuo.html

free -h;  ps aux | grep nginx
来源：http://hz.ivvv.top/gtiqzrwksm.html

[R64] 结束进程
来源：http://hz.guannengcc.top/gtsxwclfpp.html

kill -9 $(pgrep -f app.py)
来源：http://hz.fengsongda.top/gthgdcrrcb.html

[R65] 查看端口占用
来源：http://hz.gogol.net.cn/gtmcecxlij.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ydjk.org.cn/gtorsrdfsx.html

[R66] 定时任务
来源：http://hz.pycfn.com/gtinmzoanz.html

crontab -e;  crontab -l
来源：http://hz.xylfe.cn/gtwjuhzxpe.html

[R67] 生成随机十六进制串
来源：http://hz.zhoulong.xyz/gtzvltandd.html

openssl rand -hex 16
来源：http://hz.mhx1999.top/gtxuoxtfcc.html

[R68] 计算文件校验值
来源：http://hz.9152youxi.cn/gtflbypkqh.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.gotoacloud.top/gttznhcgxj.html

[R69] 生成随机密码
来源：http://hz.yuanzhike.top/gtrgkrqypr.html

head -c 16 /dev/urandom | base64
来源：http://hz.aibaodan.cn/gtpwnxwvut.html

[R70] 时间戳与互转
来源：http://hz.jqgufenzy.top/gtqopqxlrx.html

date +%s;  date -d @1700000000
来源：http://hz.zhijiandao.cn/gtppxcyieg.html

[R71] 日期格式化
来源：http://hz.sysykeji.top/gtqkjbykpz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.xuanzx.com/gtxdegsjfm.html

[R72] 等待端口就绪
来源：http://hz.nanxinkj.top/gtchghrfrv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hfpthk.cn/gtygqktkcm.html

[R73] 分割大日志
来源：http://hz.chenjidiqi.icu/gtbnevvcno.html

split -l 1000 big.log part_
来源：http://hz.jinghuilouyu.cn/gtntbqlphf.html

[R74] 批量重命名
来源：http://hz.tanke756.top/gtfrtugvyy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ivvv.top/gtirozqhwr.html

[R75] 导出环境变量
来源：http://hz.yongpay.top/gtoyrbujho.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.pycfn.com/gtueveyzda.html

[R76] 使用临时文件
来源：http://hz.gotoacloud.top/gteoanmcry.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.tian-w.cn/gtzfiwmjnf.html

[R77] 读取用户输入
来源：http://hz.kuanghao11.cn/gtrkabwiys.html

read -rp "请输入: " ans
来源：http://hz.ydjk.org.cn/gtwvtvjgst.html

[R78] 交互式菜单
来源：http://hz.ppjwa.cn/gtqueozutb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.feifeiyinyue.top/gtouoapulz.html

[R79] 解析命令行选项
来源：http://hz.gaohongyu789.top/gtqulrjbrx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jqgfzy.top/gtxbuxmyvt.html

[R80] 查看脚本执行耗时
来源：http://hz.ybcxt.top/gtbqvweluu.html

time ./run.sh
来源：http://hz.fengsongda.top/gteklwzxnk.html

================================================================================
来源：http://hz.yj202588.top/gtkkbqmvwr.html

S. C / C++ 专题
来源：http://hz.ivvv.top/gtuskxqgsy.html

================================================================================
来源：http://hz.hnqzz.top/gtizcyyuxz.html

[S01] C：Hello World
来源：http://hz.yj20258.top/gtojqcdxmh.html

#include <stdio.h>
来源：http://hz.xuanzx.com/gttwthabks.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cucudq.cn/gtmwtticrw.html

[S02] C：变量与格式化输出
来源：http://hz.jiagoushi.top/gtrqbjwxet.html

int a = 10; printf("%d\n", a);
来源：http://hz.daxiang520.top/gtqkqmbljl.html

[S03] C：读入整数
来源：http://hz.sufxvd.cn/gtazplnzwn.html

int x; scanf("%d", &x);
来源：http://hz.jinqigufen.top/gtatvrarkd.html

[S04] C：字符串复制
来源：http://hz.jinqigufen.top/gtwpdtwgcw.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.redwolf501.top/gtsbkytwdl.html

[S05] C：字符串长度
来源：http://hz.dianchejie.cn/gtrlxijcgf.html

strlen(s)
来源：http://hz.hongshengwenyu.top/gtonlccxyf.html

[S06] C：字符串比较
来源：http://hz.shanyushiyangkeji.top/gtsidluswk.html

strcmp(a, b) == 0
来源：http://hz.yueranfly.top/gtivwwbeot.html

[S07] C：数组遍历求和
来源：http://hz.snrcjt.cn/gtslkcxlpr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xylfe.cn/gtovaphfpl.html

[S08] C：动态内存分配与释放
来源：http://hz.ydjk.org.cn/gtenczzjql.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.cqqwz.cn/gthsudpfgc.html

[S09] C：结构体定义与初始化
来源：http://hz.yongpay.top/gtjyrnrykd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ehwqpu.com/gtzrwbenja.html

[S10] C：指针与解引用
来源：http://hz.andypj.xyz/gtwcefgfxm.html

int *p = &a;  *p = 5;
来源：http://hz.yueranfly.top/gtoewwilhi.html

[S11] C：逐行读文件
来源：http://hz.jinyuanbaomall.cn/gtmvzxtglf.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.shuidangran.top/gtjjlburey.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.andypj.xyz/gtemovxyds.html

fclose(f);
来源：http://hz.jinyuanbaomall.cn/gtabriaizj.html

[S12] C：写文件
来源：http://hz.shanyushiyangtech.top/gtbmvlxluh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.daxiang520.top/gtkygouepe.html

[S13] C：宏定义
来源：http://hz.tanke756.top/gtkcvijjkf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.sysykeji.top/gtidghcjhc.html

[S14] C：枚举
来源：http://hz.jianghu66.top/gtsihdqcvc.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.smart0.xyz/gtezdublid.html

[S15] C：类型转换
来源：http://hz.haohaochexian.top/gtobsdjgad.html

(double) a / b
来源：http://hz.kuanghao11.cn/gtujaaywyo.html

[S16] C：位操作置位
来源：http://hz.gaohongyu789.top/gtgjdgmljl.html

x |= (1 << 3);
来源：http://hz.smart0.xyz/gtcdoutcgb.html

[S17] C：安全拼接字符串
来源：http://hz.ivvv.top/gthhsibezr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zdqjudy.top/gtrhptiwli.html

[S18] C：命令行参数
来源：http://hz.snrcjt.cn/gtnkokedla.html

int main(int argc, char **argv)
来源：http://hz.jqgufenzy.top/gteanjoxav.html

[S19] C：快速排序
来源：http://hz.xingfuxueyuan.xyz/gtryvuknux.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.chenlongwang.top/gtpcepadlp.html

[S20] C：二分查找
来源：http://hz.xuanzx.com/gtnnejiika.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.pycfn.com/gtoyyatsii.html

[S21] C：字符类别判断
来源：http://hz.ivvv.top/gtjscantyl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xziqi.cn/gtyugnxvjf.html

[S22] C：字符串转数字
来源：http://hz.sysykeji.top/gtjntxnuzq.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.shzxlz.cn/gthrpkfkgy.html

[S23] C：随机数
来源：http://hz.zhaomingkeji.xyz/gtluwmepfq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xziqi.cn/gtypwbudnm.html

[S24] C：获取本地时间
来源：http://hz.hnxiangtu.top/gtzaazxsfu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xziqi.cn/gtvtjctlar.html

[S25] C：内存拷贝
来源：http://hz.hysaishi.cn/gtgttdjhqb.html

memcpy(dst, src, n);
来源：http://hz.52xcode.cn/gtbofjevfc.html

[S26] C：内存清零
来源：http://hz.yvedp.cn/gtiudfkwwr.html

memset(a, 0, sizeof a);
来源：http://hz.jinqigufen.top/gtpmondnkq.html

[S27] C：定义常量
来源：http://hz.9152youxi.cn/gtrhenfkbi.html

const double PI = 3.14159;
来源：http://hz.sxryk.cn/gtglaiuprw.html

[S28] C：静态变量
来源：http://hz.jiagoushi.top/gtfgnrrdxm.html

static int counter = 0;
来源：http://hz.zycfv.cn/gtifuhmnrb.html

[S29] C：变参函数
来源：http://hz.zhijiandao.cn/gtfqqobzcw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jlsjyb.cn/gtzishsibm.html

[S30] C：头文件保护
来源：http://hz.fengsongda.top/gtflnahgjs.html

#ifndef X_H
来源：http://hz.jinqigufen.top/gtqzzyvjhr.html

#define X_H
来源：http://hz.yuxming.cn/gtpkmsejhh.html

#endif
来源：http://hz.iojbl.cn/gtbhucggbi.html

[S31] C++：Hello World
来源：http://hz.ydjk.org.cn/gtnkkzmtvb.html

#include <iostream>
来源：http://hz.cqqwz.cn/gtgtcenqhy.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.daxiang520.top/gtsouqassd.html

[S32] C++：字符串
来源：http://hz.shzxlz.cn/gtixnlsoqa.html

std::string s = "hi";  s += "!";
来源：http://hz.kuanghao11.cn/gtjznjbpaa.html

[S33] C++：vector 增删
来源：http://hz.yuanzhike.top/gtruymvjjp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.pengpengdd.cyou/gthysgdglq.html

[S34] C++：遍历 vector
来源：http://hz.sufxvd.cn/gtyzbmxwyg.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.tian-w.cn/gtqyavpooo.html

[S35] C++：map
来源：http://hz.fzhhl.top/gtnvhaxhie.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinqigufen.top/gthwgwvtuc.html

[S36] C++：unordered_map
来源：http://hz.xuetiantiany.cn/gtxeqnbucn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhoulong.xyz/gtpikwsmgp.html

[S37] C++：set
来源：http://hz.aibaodan.cn/gtijceztzy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yj20258.top/gtbnqgbpdi.html

[S38] C++：排序
来源：http://hz.gzhubu.top/gtanajfqeb.html

std::sort(v.begin(), v.end());
来源：http://hz.hnqzz.top/gtrrpfjfmn.html


<!-- 参考信息 -->