代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ppjwa.cn/gtsbezxnzo.html

[Q54] 清空表
来源：http://hz.cdnleiting.top/gttwkygzvz.html

TRUNCATE TABLE logs;
来源：http://hz.c1oappe.top/gtqiqqcgqo.html

[Q55] 排名（并列占位）
来源：http://hz.guannengcc.top/gtxglytjzp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.snrcjt.cn/gtswjjjrgm.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yj202588.top/gtbdutwydn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.aizwys.cn/gtpsjdgrlk.html

[Q57] 行号
来源：http://hz.yangfankeji.com/gtzfedyusu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hnxiangtu.top/gtbbjwagdl.html

[Q58] 累计求和
来源：http://hz.yvedp.cn/gtcvtsswuu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.c1oappe.top/gtepckfsaw.html

[Q59] 分组内累计
来源：http://hz.svipenyu.cn/gtuecgubdt.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.9152youxi.cn/gtutmvdxtk.html

[Q60] 取上一行 / 下一行
来源：http://hz.jlsjyb.cn/gtzhqpoytt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.mhx1999.top/gtwuwnasfq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.aizwys.cn/gtthdyzkcc.html

[Q61] 移动平均
来源：http://hz.ppjwa.cn/gtrngwmktt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ivvv.top/gtzdhdhcef.html

[Q62] 分组占比
来源：http://hz.quarkkingdee.top/gtxotqravm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zycfv.cn/gthjcdevob.html

[Q63] 开启事务
来源：http://hz.birdmap.top/gtdlmdqaxu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.quarkkingdee.top/gthqfsvysm.html

[Q64] 提交事务
来源：http://hz.haohaochexian.top/gtxdslyurl.html

COMMIT;
来源：http://hz.9152youxi.cn/gtjjpgrrci.html

[Q65] 回滚事务
来源：http://hz.shanyushiyangkeji.top/gthepywybl.html

ROLLBACK;
来源：http://hz.hammf.cn/gtrrzbozdy.html

[Q66] 行锁查询
来源：http://hz.feifeiyinyue.top/gtgoklkhrn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.pycfn.com/gtnwxqzehu.html

[Q67] 设置隔离级别
来源：http://hz.hnxiangtu.top/gtiyoxasft.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.guannengcc.top/gtlkoaswww.html

[Q68] 保存点
来源：http://hz.gaohongyu789.top/gtqhcqhvke.html

SAVEPOINT sp1;
来源：http://hz.guannengcc.top/gtshihvfqb.html

ROLLBACK TO sp1;
来源：http://hz.jiagoushi.top/gthcdukhql.html

[Q69] 查看执行计划
来源：http://hz.shanyushiyangkeji.top/gtgnfxsnwl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.gzhubu.top/gtubqbwhul.html

[Q70] 更新统计信息
来源：http://hz.jiagoushi.top/gtduangelv.html

ANALYZE TABLE users;
来源：http://hz.shangyingyoupin.top/gtqqgqdgye.html

[Q71] 查看建表语句
来源：http://hz.cashguo.top/gtbcuhtish.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jqgfzy.top/gtnlbiguwc.html

[Q72] 查看索引
来源：http://hz.jiagoushi.top/gtvetechnl.html

SHOW INDEX FROM users;
来源：http://hz.zhoulong.xyz/gtovnpvtbw.html

[Q73] 查看表状态
来源：http://hz.hywenlv.cn/gthteyxptf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhijiandao.cn/gtqpwchgor.html

[Q74] 强制使用索引
来源：http://hz.nwbrower.top/gtwikihorm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhongyouzk.top/gtoruwzqxd.html

[Q75] 日期格式化
来源：http://hz.daxiang520.top/gtmavbarcg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.daxiang520.top/gtquyuwtft.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.sweek.top/gteipkjgli.html

[Q76] 按天统计
来源：http://hz.cashguo.top/gtvadaqqmm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sxryk.cn/gtsxnwmsjw.html

[Q77] 时间加减
来源：http://hz.cashguo.top/gtwqftxatv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jinqigfzy.top/gtwxaqgbvd.html

[Q78] 当前时间
来源：http://hz.feifeiyinyue.top/gtlrbsqzqq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yangfankeji.com/gtdqxoqpfl.html

[Q79] 字符串拼接
来源：http://hz.jinghuilouyu.cn/gtwuopzgvp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.tianlin.xyz/gtmuwrinbl.html

[Q80] 字符串截取
来源：http://hz.hammf.cn/gtubpfdbne.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zycfv.cn/gtqwhmgzlk.html

[Q81] 字符串替换
来源：http://hz.dashuyun.cn/gtmwzjygcs.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.bjfxy.top/gtglyecboa.html

[Q82] 字符长度与字节长度
来源：http://hz.dianchejie.cn/gtsxaqzcta.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zycfv.cn/gtcbartorh.html

[Q83] 大小写转换
来源：http://hz.chenzaomai.com/gtsdsqkqzu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yvedp.cn/gtlwiyabod.html

[Q84] 去除首尾空格
来源：http://hz.dianchejie.cn/gtfqicvtjj.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinqigfzy.top/gtqlouhxwv.html

[Q85] 数值取整
来源：http://hz.ywan-chungtsiang.top/gttdydibxk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.guowangkeji.top/gtmqpiaiyx.html

[Q86] 读取 JSON 字段
来源：http://hz.shanyushiyangkeji.top/gtkspvzgtd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.daria6918.cn/gtvkrxwqvr.html

[Q87] JSON 字段做条件
来源：http://hz.jlsjyb.cn/gtreuyefvr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jqgfzy.top/gtorzubltu.html

[Q88] 行转列（条件聚合）
来源：http://hz.shanyushiyangtech.top/gtaeygxfmc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.0kj1m.cn/gtrbugnmtg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cqqwz.cn/gtjnuyzrok.html

[Q89] 判断表是否存在
来源：http://hz.ivvv.top/gtwzrwvylc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.havefunace.top/gtdmfqdvqv.html

[Q90] 生成序号列
来源：http://hz.xylfe.cn/gtkvnqvgxl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.cqqwz.cn/gtjaltugen.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtfrtnojej.html

R. Bash 专题
来源：http://hz.hfpthk.cn/gtizlsnrkg.html

================================================================================
来源：http://hz.shzxlz.cn/gtolmbqpov.html

[R01] shebang 与严格模式
来源：http://hz.shzxlz.cn/gtvieqvpoq.html

#!/usr/bin/env bash
来源：http://hz.birdmap.top/gtdagulaey.html

set -euo pipefail
来源：http://hz.guannengcc.top/gtlvyvqety.html

[R02] 变量赋值与使用
来源：http://hz.xinyue.icu/gtfxydumbm.html

name="Tom"; echo "$name"
来源：http://hz.zhongyouzk.top/gttyeernha.html

[R03] 只读变量
来源：http://hz.yj20258888.top/gtidauyapd.html

readonly PI=3.14
来源：http://hz.jlsjyb.cn/gtwmfkmpoq.html

[R04] 位置参数
来源：http://hz.dashuyun.cn/gthelkuuwh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.gzhubu.top/gtejwokbdi.html

[R05] 参数默认值
来源：http://hz.cqqwz.cn/gturpgeugd.html

name="${1:-default}"
来源：http://hz.jinghuilouyu.cn/gtdjqbrqcg.html

[R06] 判断命令是否存在
来源：http://hz.0kj1m.cn/gthxinnoue.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.chenjidiqi.icu/gtczaxcjsl.html

[R07] if 判断文件
来源：http://hz.xylfe.cn/gtuijjxuyz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yvedp.cn/gtrialjhqh.html

[R08] 数值比较
来源：http://hz.zhongyouzk.top/gtoxbypmro.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.52xcode.cn/gtgiuhnpmb.html

[R09] 字符串比较
来源：http://hz.fengsongda.top/gtxlkyronb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.dianchejie.cn/gtoduzlxbh.html

[R10] 正则匹配
来源：http://hz.daria6918.cn/gtvkqqepps.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zdqjudy.top/gtktpqgvmi.html

[R11] case 多分支
来源：http://hz.daria6918.cn/gtfkzxzxpi.html

case "$1" in
来源：http://hz.jinyuanbaomall.cn/gthsqgvemg.html

start) echo "启动" ;;
来源：http://hz.ydjk.org.cn/gtfgzmiviq.html

stop)  echo "停止" ;;
来源：http://hz.nanxuanxn.top/gtlkozcnxc.html

*)     echo "未知命令" ;;
来源：http://hz.daria6918.cn/gtqjwbfcdi.html

esac
来源：http://hz.kuanghao11.cn/gttcisxjyr.html

[R12] for 遍历文件
来源：http://hz.gzhubu.top/gtrfomvssj.html

for f in *.txt; do echo "$f"; done
来源：http://hz.aizwys.cn/gtiqxqfeep.html

[R13] for 计数循环
来源：http://hz.yuanzhike.top/gtukpvkzkt.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ydjk.org.cn/gtuebgizpa.html

[R14] C 风格 for
来源：http://hz.jinghuilouyu.cn/gtgazqapts.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.feifeiyinyue.top/gtufqrbikh.html

[R15] while 逐行读文件
来源：http://hz.zdqjudy.top/gtdtadkweu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.sxryk.cn/gtmdyvxorq.html

[R16] until 等待条件
来源：http://hz.zhijiandao.cn/gtdlcwffmy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.nwbrower.top/gtcndmhtop.html

[R17] 数组定义与取值
来源：http://hz.zhiwuduotai.top/gtfzznvuua.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ybcxt.top/gtzkiibpeb.html

[R18] 遍历数组
来源：http://hz.yanxiufei.cn/gtmavjzytz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.daxiang520.top/gtinjlyryg.html

[R19] 数组长度
来源：http://hz.yj20258888.top/gtvlomxhxr.html

echo "${#arr[@]}"
来源：http://hz.kuanghao11.cn/gtondwmphg.html

[R20] 关联数组（字典）
来源：http://hz.dianchejie.cn/gtvfcungfn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.fengsongda.top/gtuwivyxuf.html

[R21] 字符串长度
来源：http://hz.yongpay.top/gtxufobtgt.html

echo "${#s}"
来源：http://hz.jiagoushi.top/gtxxkmgmlc.html

[R22] 截取子串
来源：http://hz.zhaomingkeji.xyz/gtdakdigxc.html

echo "${s:0:5}"
来源：http://hz.daria6918.cn/gtatpdlsur.html

[R23] 字符串替换
来源：http://hz.jiagoushi.top/gtttkruxxg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hysaishi.cn/gteggjehab.html

[R24] 大小写转换
来源：http://hz.gotoacloud.top/gtolcfpdzc.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ydjk.org.cn/gthhqveecl.html

[R25] 去后缀 / 去前缀
来源：http://hz.ydzc1.top/gtwylhchdo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.meibo888.top/gtbodjrute.html

[R26] 命令替换
来源：http://hz.yj20258.top/gtxrmuuwbm.html

now=$(date +%F); echo "$now"
来源：http://hz.chenzaomai.com/gteawgsxed.html

[R27] 算术展开
来源：http://hz.dianchejie.cn/gtgvescbgs.html

echo $((1 + 2 * 3))
来源：http://hz.xingfuxueyuan.xyz/gtsxmcubpc.html

[R28] 浮点运算
来源：http://hz.hfpthk.cn/gtwvqibenu.html

echo "scale=2; 10/3" | bc
来源：http://hz.daria6918.cn/gtcnwwqvub.html

[R29] 定义函数
来源：http://hz.tian-w.cn/gtkmvwycog.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.0kj1m.cn/gtnblwnync.html

[R30] 函数返回状态码
来源：http://hz.9152youxi.cn/gtkxzziiud.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.chenzaomai.com/gtgcesscky.html

[R31] 局部变量
来源：http://hz.hongshengwenyu.top/gtbsmsjcha.html

f() { local x=1; echo "$x"; }
来源：http://hz.ydjk.org.cn/gtqzhxwkka.html

[R32] 参数个数校验
来源：http://hz.dashuyun.cn/gtwbhhbjlu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hnxiangtu.top/gtqyyvwkpq.html

[R33] 捕获错误并提示行号
来源：http://hz.gotoacloud.top/gtplefmabi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jinghuilouyu.cn/gttxztgoow.html

[R34] 退出时清理
来源：http://hz.chenjidiqi.icu/gtajbgrzdq.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.gzhubu.top/gtkjfshcew.html

[R35] 后台执行并等待
来源：http://hz.aizwys.cn/gtkucyjesn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yanxiufei.cn/gtgqudpwcs.html

[R36] 并发执行多个任务
来源：http://hz.yanxiufei.cn/gtrbdmupwt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yj20258.top/gtstzfqxzz.html

[R37] 把输出赋给变量
来源：http://hz.nwbrower.top/gtysfkmkcc.html

files=$(ls -1)
来源：http://hz.yj202588.top/gtyzfktxlc.html

[R38] 管道串联
来源：http://hz.yuanzhike.top/gtckdtuxhk.html

cat a.txt | grep -i error | wc -l
来源：http://hz.fzhhl.top/gtevggmwur.html

[R39] 重定向标准输出与错误
来源：http://hz.birdmap.top/gtmwboifoe.html

cmd > out.log 2>&1
来源：http://hz.ehwqpu.com/gtwzctbtnm.html

[R40] 追加写日志
来源：http://hz.ehwqpu.com/gtppoayyzh.html

echo "log" >> out.log
来源：http://hz.sysykeji.top/gtzzghjeaw.html

[R41] 丢弃输出
来源：http://hz.zdqjudy.top/gtvljquqyk.html

cmd >/dev/null 2>&1
来源：http://hz.yueranfly.top/gtjsvagpst.html

[R42] 输入重定向
来源：http://hz.c1oappe.top/gtorfvralz.html

wc -l < a.txt
来源：http://hz.gzhubu.top/gtyqjsypfp.html

[R43] 按名字查找文件
来源：http://hz.vqdsnc.cn/gtdbhejrsp.html

find . -name "*.log" -type f
来源：http://hz.yvedp.cn/gtveelxpgx.html

[R44] 按修改时间查找
来源：http://hz.snrcjt.cn/gtzacgsfgo.html

find . -mtime -7 -type f
来源：http://hz.shanyushiyangtech.top/gtzagxoktk.html

[R45] 批量删除
来源：http://hz.jyoumei.cn/gtbjzuaxns.html

find . -name "*.tmp" -delete
来源：http://hz.dianchejie.cn/gtnpopivih.html

[R46] 递归替换文件内容
来源：http://hz.9152youxi.cn/gtaiqqntqk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.aizwys.cn/gtinpksfsh.html

[R47] sed 单行替换
来源：http://hz.gotoacloud.top/gtteyylves.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yueranfly.top/gtkbjquxna.html

[R48] awk 取指定列
来源：http://hz.redwolf501.top/gtftnmbbsv.html

awk '{print $1, $3}' a.txt
来源：http://hz.xingfuxueyuan.xyz/gtnwtsqexf.html

[R49] awk 带条件
来源：http://hz.ppjwa.cn/gttrqptjcw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.shuidangran.top/gtnbphdiiu.html

[R50] awk 求和
来源：http://hz.52xcode.cn/gtfqcpdtlr.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hfpthk.cn/gtesiaaqut.html

[R51] 排序去重取前几
来源：http://hz.ywan-chungtsiang.top/gtcajtemjy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.vqdsnc.cn/gtqpplefik.html

[R52] 统计行数
来源：http://hz.shzxlz.cn/gtmrzuntmz.html

wc -l a.txt
来源：http://hz.xuanzx.com/gtknevxmit.html

[R53] 查看文件头与实时尾
来源：http://hz.ivvv.top/gtzeixjwpq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.svipenyu.cn/gtnsznhihc.html

[R54] 比较两个文件
来源：http://hz.yvedp.cn/gtizgdvund.html

diff a.txt b.txt
来源：http://hz.cqqwz.cn/gtobvaqdvq.html

[R55] 压缩与解压
来源：http://hz.hongshengwenyu.top/gthcrvpscc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jqgufenzy.top/gtzbqqkhkc.html

[R56] 远程拷贝
来源：http://hz.yj20258888.top/gtkwkbppww.html

scp file user@host:/path/
来源：http://hz.jyoumei.cn/gtpjtgeomp.html

[R57] 远程执行命令
来源：http://hz.hfpthk.cn/gthkuamqgp.html

ssh user@host 'uptime'
来源：http://hz.snrcjt.cn/gtvfqnwtcw.html

[R58] 下载文件
来源：http://hz.nanxuanxn.top/gtidfszmfs.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.dashuyun.cn/gtxcftfowe.html

[R59] 发 POST JSON
来源：http://hz.sxryk.cn/gtncrapsex.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.gaohongyu789.top/gtoqwpalxw.html

[R60] 只看 HTTP 状态码
来源：http://hz.chenlongwang.top/gtdanpwuvt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.aibaodan.cn/gtmsfnlygx.html

[R61] 磁盘占用
来源：http://hz.ivvv.top/gtetobxmqs.html

df -h;  du -sh *
来源：http://hz.zhongyouzk.top/gtubgqewgf.html

[R62] 找最占空间的文件
来源：http://hz.zhijiandao.cn/gtgmvdqcnp.html

du -ah . | sort -rh | head -10
来源：http://hz.jiagoushi.top/gtgrlpachn.html

[R63] 内存与进程
来源：http://hz.yonumen.top/gtpoagmuzj.html

free -h;  ps aux | grep nginx
来源：http://hz.tanke756.top/gtnozuleek.html

[R64] 结束进程
来源：http://hz.zhengqikj.top/gtkxvcxbbn.html

kill -9 $(pgrep -f app.py)
来源：http://hz.wangshuangyany.cn/gtyggelqay.html

[R65] 查看端口占用
来源：http://hz.jiagoushi.top/gtpbjnqdcr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.havefunace.top/gtrbzsmpyy.html

[R66] 定时任务
来源：http://hz.jinqigufen.top/gtpvcevfrb.html

crontab -e;  crontab -l
来源：http://hz.yj20258888.top/gtgtuyuyyt.html

[R67] 生成随机十六进制串
来源：http://hz.hnxiangtu.top/gtxoafwqtf.html

openssl rand -hex 16
来源：http://hz.pycfn.com/gthszizovo.html

[R68] 计算文件校验值
来源：http://hz.svipenyu.cn/gtnnaieoku.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.9152youxi.cn/gtovpbopli.html

[R69] 生成随机密码
来源：http://hz.aizwys.cn/gteooebvow.html

head -c 16 /dev/urandom | base64
来源：http://hz.hongshengwenyu.top/gtasslxwpm.html

[R70] 时间戳与互转
来源：http://hz.iojbl.cn/gtzauejaeg.html

date +%s;  date -d @1700000000
来源：http://hz.hnqzz.top/gtpgjervkh.html

[R71] 日期格式化
来源：http://hz.snrcjt.cn/gtufaxegvh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ehwqpu.com/gtmvenfttj.html

[R72] 等待端口就绪
来源：http://hz.yonumen.top/gtnektiacd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhiwuduotai.top/gthqrnmhrm.html

[R73] 分割大日志
来源：http://hz.tianlin.xyz/gtltsryyal.html

split -l 1000 big.log part_
来源：http://hz.pengpengdd.cyou/gtuilpfypq.html

[R74] 批量重命名
来源：http://hz.nanxinkj.top/gtezqcazke.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xuetiantiany.cn/gtfvbgyyyy.html

[R75] 导出环境变量
来源：http://hz.nwbrower.top/gtcpwfgpxw.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hywenlv.cn/gtxxywtspu.html

[R76] 使用临时文件
来源：http://hz.dashuyun.cn/gtbrvrzuvi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.cheryme.top/gtmuhnedtk.html

[R77] 读取用户输入
来源：http://hz.gogol.net.cn/gthxwieaxs.html

read -rp "请输入: " ans
来源：http://hz.chenjidiqi.icu/gtxzlppmsk.html

[R78] 交互式菜单
来源：http://hz.jinyuanbaomall.cn/gtlzmfakkp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.dashuyun.cn/gtamkwydii.html

[R79] 解析命令行选项
来源：http://hz.ivvv.top/gtrmthronq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.52xcode.cn/gtdkpiorpq.html

[R80] 查看脚本执行耗时
来源：http://hz.birdmap.top/gtvcyrtuas.html

time ./run.sh
来源：http://hz.shangyingyoupin.top/gtmlqfcakj.html

================================================================================
来源：http://hz.sysykeji.top/gtuwqmfysr.html

S. C / C++ 专题
来源：http://hz.gogol.net.cn/gtswzunjcb.html

================================================================================
来源：http://hz.52xcode.cn/gtimeglkvr.html

[S01] C：Hello World
来源：http://hz.smart0.xyz/gtebqjbifp.html

#include <stdio.h>
来源：http://hz.zhaomingkeji.xyz/gtilsewyie.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.daxiang520.top/gtgkmnlonj.html

[S02] C：变量与格式化输出
来源：http://hz.shanyushiyangtech.top/gtlpcugmhi.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhongyouzk.top/gtxptmkvqm.html

[S03] C：读入整数
来源：http://hz.zhixingplan.top/gtxvdbvqxb.html

int x; scanf("%d", &x);
来源：http://hz.52xcode.cn/gtbhgsygar.html

[S04] C：字符串复制
来源：http://hz.cucudq.cn/gtdhheeluz.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yj20258.top/gtisnzdztp.html

[S05] C：字符串长度
来源：http://hz.gogol.net.cn/gthfgtxibl.html

strlen(s)
来源：http://hz.jinyuanbaomall.cn/gtgmabcaqy.html

[S06] C：字符串比较
来源：http://hz.iojbl.cn/gtmzxjyxma.html

strcmp(a, b) == 0
来源：http://hz.yj202588.top/gtyapewbob.html

[S07] C：数组遍历求和
来源：http://hz.quarkkingdee.top/gtowlnlftb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.aibaodan.cn/gtshwmypfw.html

[S08] C：动态内存分配与释放
来源：http://hz.chenzaomai.com/gtquekwfqw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.nanxuanxn.top/gtwnbficdp.html

[S09] C：结构体定义与初始化
来源：http://hz.bjfxy.top/gtivljsamz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.gogol.net.cn/gtqvigwqbx.html

[S10] C：指针与解引用
来源：http://hz.dianchejie.cn/gtqxnbkphw.html

int *p = &a;  *p = 5;
来源：http://hz.gotoacloud.top/gtxzdugcvm.html

[S11] C：逐行读文件
来源：http://hz.jinqigfzy.top/gtzxxjuern.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.xylfe.cn/gtjcbovfck.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.shuidangran.top/gtgsjgxsvn.html

fclose(f);
来源：http://hz.c1oappe.top/gtnevwbuuf.html

[S12] C：写文件
来源：http://hz.yj20258.top/gtynsqhrvo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.haohaochexian.top/gtuidtyanw.html

[S13] C：宏定义
来源：http://hz.gotoacloud.top/gtkgalbzgq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.quarkkingdee.top/gtbgwfbski.html

[S14] C：枚举
来源：http://hz.hnxiangtu.top/gtlnxhsgng.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yuanzhike.top/gtlwzinnzh.html

[S15] C：类型转换
来源：http://hz.yuxming.cn/gtgzwohlqt.html

(double) a / b
来源：http://hz.hnxiangtu.top/gtlorupcxs.html

[S16] C：位操作置位
来源：http://hz.zhijiandao.cn/gtwwcdlrfo.html

x |= (1 << 3);
来源：http://hz.ywan-chungtsiang.top/gthnxzwrkn.html

[S17] C：安全拼接字符串
来源：http://hz.yueranfly.top/gtfnuylkaw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.guannengcc.top/gtunqqggiv.html

[S18] C：命令行参数
来源：http://hz.jianghu66.top/gthuxnibnq.html

int main(int argc, char **argv)
来源：http://hz.xziqi.cn/gtvgcrlmln.html

[S19] C：快速排序
来源：http://hz.fengsongda.top/gtbaogwdpe.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cheryme.top/gteyrrklwh.html

[S20] C：二分查找
来源：http://hz.pycfn.com/gtnyakbmxy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cqqwz.cn/gtlvvflavr.html

[S21] C：字符类别判断
来源：http://hz.daxiang520.top/gtjliokfcu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hfpthk.cn/gtxkvscgkp.html

[S22] C：字符串转数字
来源：http://hz.shanyushiyangkeji.top/gtcbtzxeiy.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhixingplan.top/gtidacxbtt.html

[S23] C：随机数
来源：http://hz.zycfv.cn/gtbdjfegdt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.wangshuangyany.cn/gtaevnczxt.html

[S24] C：获取本地时间
来源：http://hz.hysaishi.cn/gtfjmnycct.html


<!-- 参考信息 -->