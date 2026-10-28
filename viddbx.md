代发 wailian999

[Q44] IN 子查询
来源：http://hz.ybcxt.top/gtzzwscgwu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.gzhubu.top/gtkoarwele.html

[Q45] EXISTS 判断存在
来源：http://hz.daxiang520.top/gtamwjcgcu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.mhx1999.top/gtygabbrub.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.kuanghao11.cn/gtfecftnok.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhengqikj.top/gtanamqaep.html

[Q47] 与平均值比较
来源：http://hz.guowangkeji.top/gtdppndvkt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yonumen.top/gtlxmdzocy.html

[Q48] CTE 公用表表达式
来源：http://hz.cashguo.top/gttkrafqkn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.gzhubu.top/gtuufohwjr.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.fengsongda.top/gtrbuspqlv.html

[Q49] 更新单行
来源：http://hz.meibo888.top/gtwecpllbq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jyoumei.cn/gtezvqlyay.html

[Q50] 批量更新
来源：http://hz.xziqi.cn/gtuoenepeo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.cashguo.top/gtadounzuv.html

[Q51] 用子查询更新
来源：http://hz.dianchejie.cn/gtgrirfhhb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ywan-chungtsiang.top/gtcimdxcku.html

[Q52] 删除指定行
来源：http://hz.0kj1m.cn/gtasvichmj.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ydjk.org.cn/gtjclexfya.html

[Q53] 按条件删除
来源：http://hz.316326.xyz/gtdduxxlmm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.sxryk.cn/gtdatoyraj.html

[Q54] 清空表
来源：http://hz.cdnleiting.top/gtgqxlrpjf.html

TRUNCATE TABLE logs;
来源：http://hz.nanxinkj.top/gtwsvyzkba.html

[Q55] 排名（并列占位）
来源：http://hz.nwbrower.top/gtnuhpzrjd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yangfankeji.com/gtsppywxzo.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jinghuilouyu.cn/gthsvgsxmm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.daxiang520.top/gtaskpvtqg.html

[Q57] 行号
来源：http://hz.vqdsnc.cn/gtcwkshcqr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.wangshuangyany.cn/gtbbuwvfku.html

[Q58] 累计求和
来源：http://hz.shzxlz.cn/gtnujvuegd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.meibo888.top/gtudxkrzfm.html

[Q59] 分组内累计
来源：http://hz.iojbl.cn/gtgdaekeiy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.xziqi.cn/gtiatfhflv.html

[Q60] 取上一行 / 下一行
来源：http://hz.nanxuanxn.top/gtdzprjcnh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.wangdashe.top/gtwonekwbn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.aizwys.cn/gtodtakmhq.html

[Q61] 移动平均
来源：http://hz.jlsjyb.cn/gtnculqyal.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.tian-w.cn/gtoncucfhu.html

[Q62] 分组占比
来源：http://hz.snrcjt.cn/gtcyrrfnor.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhixingplan.top/gtifowongg.html

[Q63] 开启事务
来源：http://hz.vqdsnc.cn/gtahvkrfzm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hammf.cn/gtayxagwla.html

[Q64] 提交事务
来源：http://hz.hnxiangtu.top/gtecxxhilc.html

COMMIT;
来源：http://hz.daxiang520.top/gtabnzmakp.html

[Q65] 回滚事务
来源：http://hz.ydjk.org.cn/gtuyioxdeg.html

ROLLBACK;
来源：http://hz.shuidangran.top/gtsyyohpts.html

[Q66] 行锁查询
来源：http://hz.cdnleiting.top/gtaonetgcd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.shanyushiyangtech.top/gtggrxdceq.html

[Q67] 设置隔离级别
来源：http://hz.bjfxy.top/gtuqsdkvho.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.shanyushiyangtech.top/gtqjioefxn.html

[Q68] 保存点
来源：http://hz.nanxinkj.top/gtjlamsari.html

SAVEPOINT sp1;
来源：http://hz.c1oappe.top/gtkeqerhwl.html

ROLLBACK TO sp1;
来源：http://hz.pengpengdd.cyou/gtdojfpgzq.html

[Q69] 查看执行计划
来源：http://hz.jinqigfzy.top/gtmqvcblxu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.redwolf501.top/gtdakjbkml.html

[Q70] 更新统计信息
来源：http://hz.feifeiyinyue.top/gtavqxcdsm.html

ANALYZE TABLE users;
来源：http://hz.hywenlv.cn/gtviljxyfa.html

[Q71] 查看建表语句
来源：http://hz.wangshuangyany.cn/gtgitoebuy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hnxiangtu.top/gtcbjcoeaw.html

[Q72] 查看索引
来源：http://hz.bjfxy.top/gtvefvvlta.html

SHOW INDEX FROM users;
来源：http://hz.sufxvd.cn/gtgjtvxxne.html

[Q73] 查看表状态
来源：http://hz.yj20258.top/gtqnxqhdul.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hnxiangtu.top/gtoxqjgrkk.html

[Q74] 强制使用索引
来源：http://hz.9152youxi.cn/gtjutywino.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.ywan-chungtsiang.top/gtdrxwksmg.html

[Q75] 日期格式化
来源：http://hz.cucudq.cn/gtydfxenuy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ydzc1.top/gtccvflmhj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.tian-w.cn/gtpftetfzy.html

[Q76] 按天统计
来源：http://hz.shangyingyoupin.top/gtgmwfmypf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shangyingyoupin.top/gtuykceswa.html

[Q77] 时间加减
来源：http://hz.tanke756.top/gtkzdcyniy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zdqjudy.top/gthpvsrrtv.html

[Q78] 当前时间
来源：http://hz.cqqwz.cn/gtqybntkya.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.andypj.xyz/gtlbfqpwji.html

[Q79] 字符串拼接
来源：http://hz.jlsjyb.cn/gtufjvjwbw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.meibo888.top/gtkcrqfihs.html

[Q80] 字符串截取
来源：http://hz.cheryme.top/gtfydfklsa.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jqgufenzy.top/gtwcdoesow.html

[Q81] 字符串替换
来源：http://hz.jqgfzy.top/gtjjvcvaxr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.cdnleiting.top/gtqrhwrohd.html

[Q82] 字符长度与字节长度
来源：http://hz.9152youxi.cn/gthehotvrd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.0kj1m.cn/gtctljgoxu.html

[Q83] 大小写转换
来源：http://hz.hongshengwenyu.top/gtbbyrzscl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.chenzaomai.com/gtmjbgsvib.html

[Q84] 去除首尾空格
来源：http://hz.zhijiandao.cn/gtavpkttyf.html

SELECT TRIM(name) FROM users;
来源：http://hz.shanyushiyangtech.top/gtzldcwdwn.html

[Q85] 数值取整
来源：http://hz.daxiang520.top/gtbnhmltee.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.9152youxi.cn/gtvfjdqnxg.html

[Q86] 读取 JSON 字段
来源：http://hz.yongpay.top/gtxtoxbrai.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jlsjyb.cn/gtdwxteset.html

[Q87] JSON 字段做条件
来源：http://hz.shzxlz.cn/gtinshvnwv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xuanzx.com/gtbewtczin.html

[Q88] 行转列（条件聚合）
来源：http://hz.hnqzz.top/gtieqxfrxk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.shuidangran.top/gtnzzzlmoy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ivvv.top/gtgbogmilj.html

[Q89] 判断表是否存在
来源：http://hz.ydjk.org.cn/gtcymgscuw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yuxming.cn/gtclmihxbj.html

[Q90] 生成序号列
来源：http://hz.haohaochexian.top/gthggsxvlt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yangfankeji.com/gtpfceumnv.html

================================================================================
来源：http://hz.chenlongwang.top/gtxxcvqlrr.html

R. Bash 专题
来源：http://hz.daxiang520.top/gtjdciovbo.html

================================================================================
来源：http://hz.dashuyun.cn/gtnnrcpqom.html

[R01] shebang 与严格模式
来源：http://hz.yj202588.top/gtrugmyczb.html

#!/usr/bin/env bash
来源：http://hz.yj202588.top/gtibrynhvm.html

set -euo pipefail
来源：http://hz.ybcxt.top/gtdwltuhbu.html

[R02] 变量赋值与使用
来源：http://hz.jinqigufen.top/gtlngdyfit.html

name="Tom"; echo "$name"
来源：http://hz.ehwqpu.com/gtmqribwqy.html

[R03] 只读变量
来源：http://hz.hammf.cn/gtwaljsphr.html

readonly PI=3.14
来源：http://hz.bjfxy.top/gtjecrkwjl.html

[R04] 位置参数
来源：http://hz.tian-w.cn/gtfdedhckr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hysaishi.cn/gtubuarxpf.html

[R05] 参数默认值
来源：http://hz.zhiwuduotai.top/gtdowdckwq.html

name="${1:-default}"
来源：http://hz.gzhubu.top/gtdrlfctjs.html

[R06] 判断命令是否存在
来源：http://hz.ydzc1.top/gtofgsrkfc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.birdmap.top/gtsybpsmiz.html

[R07] if 判断文件
来源：http://hz.sufxvd.cn/gtveuwnrnz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.sysykeji.top/gtcwuahmuf.html

[R08] 数值比较
来源：http://hz.shzxlz.cn/gttaskjmsb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.hywenlv.cn/gtaxwusotf.html

[R09] 字符串比较
来源：http://hz.xuanzx.com/gtphjxvmsm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.shanyushiyangkeji.top/gtevlsbkso.html

[R10] 正则匹配
来源：http://hz.vqdsnc.cn/gtkoyavexs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhengqikj.top/gtckgkxfmu.html

[R11] case 多分支
来源：http://hz.yueranfly.top/gtynpqrqdv.html

case "$1" in
来源：http://hz.sufxvd.cn/gthzlakvhz.html

start) echo "启动" ;;
来源：http://hz.yj202588.top/gtguvvksvp.html

stop)  echo "停止" ;;
来源：http://hz.ydjk.org.cn/gtndgwrbof.html

*)     echo "未知命令" ;;
来源：http://hz.xinyue.icu/gtkfnjivcy.html

esac
来源：http://hz.cqqwz.cn/gtkstxrewn.html

[R12] for 遍历文件
来源：http://hz.52xcode.cn/gtwwlvduyj.html

for f in *.txt; do echo "$f"; done
来源：http://hz.sysykeji.top/gtoveecbxf.html

[R13] for 计数循环
来源：http://hz.fzhhl.top/gtnyhqwaxc.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jqgufenzy.top/gtlvujgifh.html

[R14] C 风格 for
来源：http://hz.meibo888.top/gtqrrxiatk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yj202588.top/gtmwbayzun.html

[R15] while 逐行读文件
来源：http://hz.hywenlv.cn/gtggaqueqt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yongpay.top/gtkpfrcwet.html

[R16] until 等待条件
来源：http://hz.hfpthk.cn/gtokoeanlo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhijiandao.cn/gtnbqyargb.html

[R17] 数组定义与取值
来源：http://hz.guannengcc.top/gtandjnsgx.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.chenlongwang.top/gtpsouckzd.html

[R18] 遍历数组
来源：http://hz.fengsongda.top/gtzxtsmsfk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.c1oappe.top/gtmlpdkkpu.html

[R19] 数组长度
来源：http://hz.jiagoushi.top/gthkmggkam.html

echo "${#arr[@]}"
来源：http://hz.mhx1999.top/gtbvisuotw.html

[R20] 关联数组（字典）
来源：http://hz.kuanghao11.cn/gtkahbyeof.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.vqdsnc.cn/gtbnuskvcr.html

[R21] 字符串长度
来源：http://hz.hnqzz.top/gtkgezkgas.html

echo "${#s}"
来源：http://hz.guowangkeji.top/gtsunxvgot.html

[R22] 截取子串
来源：http://hz.hnqzz.top/gtevtupywi.html

echo "${s:0:5}"
来源：http://hz.pengpengdd.cyou/gtytmxisbz.html

[R23] 字符串替换
来源：http://hz.9152youxi.cn/gtwvlksipu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.316326.xyz/gtguzqumwn.html

[R24] 大小写转换
来源：http://hz.0kj1m.cn/gtexzyciys.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hammf.cn/gtwflykqak.html

[R25] 去后缀 / 去前缀
来源：http://hz.xuetiantiany.cn/gtgyckvdlt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.birdmap.top/gtmdckwfms.html

[R26] 命令替换
来源：http://hz.xylfe.cn/gtzhrsgfxs.html

now=$(date +%F); echo "$now"
来源：http://hz.zdqjudy.top/gtzodkuleu.html

[R27] 算术展开
来源：http://hz.meibo888.top/gtkwmsdvet.html

echo $((1 + 2 * 3))
来源：http://hz.pycfn.com/gtzhvfcibu.html

[R28] 浮点运算
来源：http://hz.dianchejie.cn/gtmayjxhme.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhiwuduotai.top/gtmbeqjmrm.html

[R29] 定义函数
来源：http://hz.jinqigufen.top/gtzrrmgznw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jinqigfzy.top/gtnugryifi.html

[R30] 函数返回状态码
来源：http://hz.cdnleiting.top/gtmegvjtez.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.aibaodan.cn/gtlcgmxtsf.html

[R31] 局部变量
来源：http://hz.jinqigfzy.top/gthatxntgm.html

f() { local x=1; echo "$x"; }
来源：http://hz.guowangkeji.top/gtfqokxwgj.html

[R32] 参数个数校验
来源：http://hz.xuetiantiany.cn/gthgraehtx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.guowangkeji.top/gtuzxrwvrb.html

[R33] 捕获错误并提示行号
来源：http://hz.xingfuxueyuan.xyz/gtvdxhmovw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.haohaochexian.top/gtvumhwvmq.html

[R34] 退出时清理
来源：http://hz.ywan-chungtsiang.top/gtvhnrchpm.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.havefunace.top/gtyqetcwkd.html

[R35] 后台执行并等待
来源：http://hz.meibo888.top/gtgxwunryq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.dashuyun.cn/gtlqqfiiwx.html

[R36] 并发执行多个任务
来源：http://hz.cdnleiting.top/gtpefweaks.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yuanzhike.top/gtfnuvocku.html

[R37] 把输出赋给变量
来源：http://hz.pycfn.com/gtvklgftch.html

files=$(ls -1)
来源：http://hz.pengpengdd.cyou/gtnynkyrsd.html

[R38] 管道串联
来源：http://hz.ydzc1.top/gtdyiuxspa.html

cat a.txt | grep -i error | wc -l
来源：http://hz.chenzaomai.com/gtzvlrasqf.html

[R39] 重定向标准输出与错误
来源：http://hz.andypj.xyz/gtkrmqlfot.html

cmd > out.log 2>&1
来源：http://hz.zhaomingkeji.xyz/gtutoxfgfy.html

[R40] 追加写日志
来源：http://hz.feifeiyinyue.top/gtuuprkvrj.html

echo "log" >> out.log
来源：http://hz.aibaodan.cn/gtwifotoqn.html

[R41] 丢弃输出
来源：http://hz.meibo888.top/gtyzmfyomj.html

cmd >/dev/null 2>&1
来源：http://hz.shanyushiyangkeji.top/gtmmxgqhmt.html

[R42] 输入重定向
来源：http://hz.chenlongwang.top/gtdcrfglhb.html

wc -l < a.txt
来源：http://hz.daxiang520.top/gtdhnxhijw.html

[R43] 按名字查找文件
来源：http://hz.cqqwz.cn/gtgczriomp.html

find . -name "*.log" -type f
来源：http://hz.jlsjyb.cn/gtvplylkcs.html

[R44] 按修改时间查找
来源：http://hz.zhixingplan.top/gtgachelxt.html

find . -mtime -7 -type f
来源：http://hz.yvedp.cn/gtbvdvhmdm.html

[R45] 批量删除
来源：http://hz.daria6918.cn/gtkapgctkr.html

find . -name "*.tmp" -delete
来源：http://hz.wangdashe.top/gtlkcjyfzj.html

[R46] 递归替换文件内容
来源：http://hz.cqqwz.cn/gtkdjmmqki.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.smart0.xyz/gtgggbkahc.html

[R47] sed 单行替换
来源：http://hz.tian-w.cn/gthemaccpq.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hfpthk.cn/gtuatpjtik.html

[R48] awk 取指定列
来源：http://hz.jinyuanbaomall.cn/gtekjapxez.html

awk '{print $1, $3}' a.txt
来源：http://hz.jqgufenzy.top/gtoefwiuwt.html

[R49] awk 带条件
来源：http://hz.shuidangran.top/gtwppuscil.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xinyue.icu/gtjjxrvkfu.html

[R50] awk 求和
来源：http://hz.jianghu66.top/gteackeocq.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jyoumei.cn/gtkzjgxqdo.html

[R51] 排序去重取前几
来源：http://hz.xuanzx.com/gtslroqqlx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhiwuduotai.top/gtnunhteyx.html

[R52] 统计行数
来源：http://hz.yanxiufei.cn/gtbnmaeypa.html

wc -l a.txt
来源：http://hz.hammf.cn/gtadlylkrf.html

[R53] 查看文件头与实时尾
来源：http://hz.aibaodan.cn/gtfjkyngut.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zdqjudy.top/gturtqvbcf.html

[R54] 比较两个文件
来源：http://hz.fzhhl.top/gtusvaowdp.html

diff a.txt b.txt
来源：http://hz.cashguo.top/gtmwiildxw.html

[R55] 压缩与解压
来源：http://hz.zycfv.cn/gtmgxyiyyn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.fzhhl.top/gtuzitsfyt.html

[R56] 远程拷贝
来源：http://hz.daxiang520.top/gtfteazqmm.html

scp file user@host:/path/
来源：http://hz.cqqwz.cn/gthjqqtxhc.html

[R57] 远程执行命令
来源：http://hz.tanke756.top/gtxvajdejj.html

ssh user@host 'uptime'
来源：http://hz.cucudq.cn/gtoflxsjjy.html

[R58] 下载文件
来源：http://hz.hongshengwenyu.top/gtipojsdnh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.tanke756.top/gtqsbsoozc.html

[R59] 发 POST JSON
来源：http://hz.iojbl.cn/gtqliovuaf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.tian-w.cn/gtjiysknjv.html

[R60] 只看 HTTP 状态码
来源：http://hz.bjfxy.top/gtfnfnasne.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhengqikj.top/gtiwforgnv.html

[R61] 磁盘占用
来源：http://hz.hongshengwenyu.top/gtnszrxjdg.html

df -h;  du -sh *
来源：http://hz.yangfankeji.com/gtbfoallgv.html

[R62] 找最占空间的文件
来源：http://hz.yanxiufei.cn/gtlebsxcui.html

du -ah . | sort -rh | head -10
来源：http://hz.cdnleiting.top/gtnabinzco.html

[R63] 内存与进程
来源：http://hz.zhaomingkeji.xyz/gtxepatvil.html

free -h;  ps aux | grep nginx
来源：http://hz.gaohongyu789.top/gtblfjvjlq.html

[R64] 结束进程
来源：http://hz.guowangkeji.top/gtdptmnasq.html

kill -9 $(pgrep -f app.py)
来源：http://hz.xziqi.cn/gtliocduse.html

[R65] 查看端口占用
来源：http://hz.vqdsnc.cn/gthlwhdjqp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.fzhhl.top/gtwlvzlxxy.html

[R66] 定时任务
来源：http://hz.xingfuxueyuan.xyz/gtbjxaqejy.html

crontab -e;  crontab -l
来源：http://hz.ydjk.org.cn/gtpmkqnmct.html

[R67] 生成随机十六进制串
来源：http://hz.zhaomingkeji.xyz/gtukwchtqo.html

openssl rand -hex 16
来源：http://hz.dianchejie.cn/gtngagwnqw.html

[R68] 计算文件校验值
来源：http://hz.xuanzx.com/gtbuyvzemu.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cdnleiting.top/gtaknzvwkt.html

[R69] 生成随机密码
来源：http://hz.hywenlv.cn/gtewspcoal.html

head -c 16 /dev/urandom | base64
来源：http://hz.316326.xyz/gtbyzzsaxf.html

[R70] 时间戳与互转
来源：http://hz.yangfankeji.com/gtagpyrqwu.html

date +%s;  date -d @1700000000
来源：http://hz.tianlin.xyz/gtlksxnwqe.html

[R71] 日期格式化
来源：http://hz.pycfn.com/gteqcbbref.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.haohaochexian.top/gtphqbijtd.html

[R72] 等待端口就绪
来源：http://hz.ydjk.org.cn/gtfmtrblsn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhongyouzk.top/gtozkvwzfe.html

[R73] 分割大日志
来源：http://hz.jinqigufen.top/gtmbutcwps.html

split -l 1000 big.log part_
来源：http://hz.svipenyu.cn/gtwgvrmrjp.html

[R74] 批量重命名
来源：http://hz.andypj.xyz/gtpeihyxoc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.andypj.xyz/gtjfhmlrwf.html

[R75] 导出环境变量
来源：http://hz.xinyue.icu/gtsxevqkag.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.52xcode.cn/gtjorbwoze.html

[R76] 使用临时文件
来源：http://hz.zhaomingkeji.xyz/gtfqxkcjvs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yvedp.cn/gtfncvlxzd.html

[R77] 读取用户输入
来源：http://hz.yuanzhike.top/gtdzrslyin.html

read -rp "请输入: " ans
来源：http://hz.zhengqikj.top/gtkmdolzpr.html

[R78] 交互式菜单
来源：http://hz.yuanzhike.top/gtpepqfbwl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xziqi.cn/gtewdihzcw.html

[R79] 解析命令行选项
来源：http://hz.shanyushiyangtech.top/gtolbilmlh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.pengpengdd.cyou/gtqkvarobf.html

[R80] 查看脚本执行耗时
来源：http://hz.hnqzz.top/gtebupegxw.html

time ./run.sh
来源：http://hz.shuidangran.top/gtqxztphep.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtaeldxwup.html

S. C / C++ 专题
来源：http://hz.ybcxt.top/gtyvjfwytl.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtwciljjmb.html

[S01] C：Hello World
来源：http://hz.vqdsnc.cn/gthmlklyfx.html

#include <stdio.h>
来源：http://hz.birdmap.top/gtviinxned.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.aizwys.cn/gtypqomzil.html

[S02] C：变量与格式化输出
来源：http://hz.hnqzz.top/gtocotqnkh.html

int a = 10; printf("%d\n", a);
来源：http://hz.shuidangran.top/gtqcrlkhgn.html

[S03] C：读入整数
来源：http://hz.yueranfly.top/gtdbkacaif.html

int x; scanf("%d", &x);
来源：http://hz.xylfe.cn/gtzjribelb.html

[S04] C：字符串复制
来源：http://hz.zhengqikj.top/gtgcddorov.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.chenzaomai.com/gtxxrmieba.html

[S05] C：字符串长度
来源：http://hz.yonumen.top/gthwonrenb.html

strlen(s)
来源：http://hz.gzhubu.top/gtspwnhqmr.html

[S06] C：字符串比较
来源：http://hz.shangyingyoupin.top/gtgbpgaoak.html

strcmp(a, b) == 0
来源：http://hz.havefunace.top/gtbnijtnia.html

[S07] C：数组遍历求和
来源：http://hz.pycfn.com/gtaafjdgfx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.sysykeji.top/gtofhglkiy.html

[S08] C：动态内存分配与释放
来源：http://hz.daria6918.cn/gtwrtwjame.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ehwqpu.com/gtgprmhhif.html

[S09] C：结构体定义与初始化
来源：http://hz.jqgufenzy.top/gtcqmvucus.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.pengpengdd.cyou/gtgcsfluir.html

[S10] C：指针与解引用
来源：http://hz.chenzaomai.com/gtgzduwixi.html

int *p = &a;  *p = 5;
来源：http://hz.svipenyu.cn/gtapwcvetq.html

[S11] C：逐行读文件
来源：http://hz.316326.xyz/gttmnwsrsz.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jqgfzy.top/gttlxrzzlp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jianghu66.top/gtqjbsvhpa.html

fclose(f);
来源：http://hz.bjfxy.top/gtepldkxor.html

[S12] C：写文件
来源：http://hz.hnqzz.top/gtmbckauje.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xuetiantiany.cn/gtgknpyrzy.html

[S13] C：宏定义
来源：http://hz.jinqigufen.top/gtuhysepfo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.andypj.xyz/gtakvtgccy.html

[S14] C：枚举
来源：http://hz.sufxvd.cn/gtdttmmvrp.html


<!-- 参考信息 -->