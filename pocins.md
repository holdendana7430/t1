代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://hz.daxiang520.top/gtquthqvca.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.gotoacloud.top/gtxfkjzdyp.html

[Q43] 标量子查询
来源：http://hz.guannengcc.top/gtfetxgcuh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.gzhubu.top/gtyhdfxjhf.html

[Q44] IN 子查询
来源：http://hz.xylfe.cn/gtngrighhg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.0kj1m.cn/gtkngzpvlf.html

[Q45] EXISTS 判断存在
来源：http://hz.ppjwa.cn/gtewiksbik.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gaohongyu789.top/gtuswrtpfs.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.chenlongwang.top/gtqryuovpx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.fzhhl.top/gtpgvfqnvs.html

[Q47] 与平均值比较
来源：http://hz.aizwys.cn/gtddmfwzxv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.cashguo.top/gtgidymgqp.html

[Q48] CTE 公用表表达式
来源：http://hz.guannengcc.top/gttdexqnxd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.quarkkingdee.top/gtrsuqrqbk.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.nanxuanxn.top/gthuvjqsjq.html

[Q49] 更新单行
来源：http://hz.ppjwa.cn/gtscjtvbrs.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jinghuilouyu.cn/gtpdnrwhgx.html

[Q50] 批量更新
来源：http://hz.redwolf501.top/gtecrpoppw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.pengpengdd.cyou/gtegnkcfsj.html

[Q51] 用子查询更新
来源：http://hz.kuanghao11.cn/gtfgabmpkd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.gaohongyu789.top/gtiahrzfuf.html

[Q52] 删除指定行
来源：http://hz.gotoacloud.top/gtoixgsuzm.html

DELETE FROM users WHERE id = 10;
来源：http://hz.tian-w.cn/gtyjnnpfsi.html

[Q53] 按条件删除
来源：http://hz.yongpay.top/gtpdpuiqgj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ydjk.org.cn/gtltjzlcgy.html

[Q54] 清空表
来源：http://hz.daria6918.cn/gtolvrciic.html

TRUNCATE TABLE logs;
来源：http://hz.chenzaomai.com/gtmwwdbkcg.html

[Q55] 排名（并列占位）
来源：http://hz.jinghuilouyu.cn/gtazaxbqrb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hywenlv.cn/gtrvywrpjv.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jqgfzy.top/gtrysnizyw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yueranfly.top/gtqbqhohat.html

[Q57] 行号
来源：http://hz.zhixingplan.top/gtfqqkxjeh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jlsjyb.cn/gtjrxbaetv.html

[Q58] 累计求和
来源：http://hz.wangdashe.top/gtlebpqagf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yuxming.cn/gtfsyovdxb.html

[Q59] 分组内累计
来源：http://hz.tian-w.cn/gtepdtoqxe.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yuxming.cn/gttpxnuhti.html

[Q60] 取上一行 / 下一行
来源：http://hz.shuidangran.top/gtxntrbalk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jqgufenzy.top/gtuvnhgsca.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.havefunace.top/gtcxifubzm.html

[Q61] 移动平均
来源：http://hz.tianlin.xyz/gtdopayzyw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shanyushiyangkeji.top/gtdnimdlsw.html

[Q62] 分组占比
来源：http://hz.zycfv.cn/gthmwvprnh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhixingplan.top/gtnxjvejhg.html

[Q63] 开启事务
来源：http://hz.ybcxt.top/gtdjvvjxoy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.snrcjt.cn/gtcoctklvy.html

[Q64] 提交事务
来源：http://hz.pengpengdd.cyou/gtcflrimlj.html

COMMIT;
来源：http://hz.zycfv.cn/gtdqwcbudf.html

[Q65] 回滚事务
来源：http://hz.daria6918.cn/gtxhzynptt.html

ROLLBACK;
来源：http://hz.iojbl.cn/gthzsppibk.html

[Q66] 行锁查询
来源：http://hz.9152youxi.cn/gtxcscrjzu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yj20258888.top/gtqyopshdk.html

[Q67] 设置隔离级别
来源：http://hz.wangshuangyany.cn/gtvefskhqv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ehwqpu.com/gttzmbzsxi.html

[Q68] 保存点
来源：http://hz.ppjwa.cn/gtzcgnnqoz.html

SAVEPOINT sp1;
来源：http://hz.daria6918.cn/gtmaxbzdlw.html

ROLLBACK TO sp1;
来源：http://hz.c1oappe.top/gtjgxnsmlk.html

[Q69] 查看执行计划
来源：http://hz.gaohongyu789.top/gtnqfowmzj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.fengsongda.top/gthkccqbso.html

[Q70] 更新统计信息
来源：http://hz.chenlongwang.top/gtbenyzahr.html

ANALYZE TABLE users;
来源：http://hz.cqqwz.cn/gtlipzfiuc.html

[Q71] 查看建表语句
来源：http://hz.yueranfly.top/gtbauyltmd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jinghuilouyu.cn/gtnjptdeiu.html

[Q72] 查看索引
来源：http://hz.pengpengdd.cyou/gtqctfvyhv.html

SHOW INDEX FROM users;
来源：http://hz.birdmap.top/gtwdgnpjyu.html

[Q73] 查看表状态
来源：http://hz.zhixingplan.top/gtygwoaucn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.shuidangran.top/gtdhygqeic.html

[Q74] 强制使用索引
来源：http://hz.ydzc1.top/gtpjkbikoo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.cqqwz.cn/gtstphhhyy.html

[Q75] 日期格式化
来源：http://hz.zhengqikj.top/gtevocpqjt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ydzc1.top/gtpcmmtfno.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ppjwa.cn/gtjxrcxnyr.html

[Q76] 按天统计
来源：http://hz.jianghu66.top/gtfehqrzqt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yuanzhike.top/gtrozrcphz.html

[Q77] 时间加减
来源：http://hz.pycfn.com/gttnxscgnc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jlsjyb.cn/gtjhhfmfly.html

[Q78] 当前时间
来源：http://hz.fengsongda.top/gtoslztauz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.ydzc1.top/gtcwcgxcao.html

[Q79] 字符串拼接
来源：http://hz.ivvv.top/gtqpwqgfik.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.dashuyun.cn/gtvaghtbub.html

[Q80] 字符串截取
来源：http://hz.zhongyouzk.top/gtzjkxyyxx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.hnqzz.top/gtjidymlzp.html

[Q81] 字符串替换
来源：http://hz.jiagoushi.top/gtvaclcqgg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.chenlongwang.top/gtzximozcz.html

[Q82] 字符长度与字节长度
来源：http://hz.ybcxt.top/gtgciftgso.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.9152youxi.cn/gtnncvracx.html

[Q83] 大小写转换
来源：http://hz.sweek.top/gtdigsamxu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xziqi.cn/gtxgjvcclj.html

[Q84] 去除首尾空格
来源：http://hz.jianghu66.top/gtligbdtul.html

SELECT TRIM(name) FROM users;
来源：http://hz.0kj1m.cn/gtzuklraiz.html

[Q85] 数值取整
来源：http://hz.jyoumei.cn/gtejwvidcj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.aibaodan.cn/gteumiaspl.html

[Q86] 读取 JSON 字段
来源：http://hz.guowangkeji.top/gtxjtyfyam.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jinghuilouyu.cn/gtvftkjsaz.html

[Q87] JSON 字段做条件
来源：http://hz.daxiang520.top/gtnldkccsk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.meibo888.top/gtqrjghmax.html

[Q88] 行转列（条件聚合）
来源：http://hz.andypj.xyz/gtqwmhyija.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhengqikj.top/gtrlxcxden.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhoulong.xyz/gthgkecozf.html

[Q89] 判断表是否存在
来源：http://hz.hywenlv.cn/gtwlfzwohk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ydjk.org.cn/gtbjwnywaq.html

[Q90] 生成序号列
来源：http://hz.tianlin.xyz/gtabekjyxn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.pycfn.com/gtospdtopd.html

================================================================================
来源：http://hz.cqqwz.cn/gtytjupzss.html

R. Bash 专题
来源：http://hz.yuanzhike.top/gtxzdjpikp.html

================================================================================
来源：http://hz.snrcjt.cn/gtiezhfqud.html

[R01] shebang 与严格模式
来源：http://hz.gotoacloud.top/gtmgbppgry.html

#!/usr/bin/env bash
来源：http://hz.dashuyun.cn/gtyqriemtl.html

set -euo pipefail
来源：http://hz.pengpengdd.cyou/gtdgdlmrcz.html

[R02] 变量赋值与使用
来源：http://hz.jlsjyb.cn/gtbenatzze.html

name="Tom"; echo "$name"
来源：http://hz.andypj.xyz/gtuxzxvbja.html

[R03] 只读变量
来源：http://hz.gzhubu.top/gtsmzqcdes.html

readonly PI=3.14
来源：http://hz.jiagoushi.top/gtbdudvvps.html

[R04] 位置参数
来源：http://hz.chenlongwang.top/gtpnmbrfkk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.pengpengdd.cyou/gtrukwgbmm.html

[R05] 参数默认值
来源：http://hz.iojbl.cn/gtziwqpsuz.html

name="${1:-default}"
来源：http://hz.zdqjudy.top/gtvnydtkkr.html

[R06] 判断命令是否存在
来源：http://hz.svipenyu.cn/gtqauyagcz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jinyuanbaomall.cn/gtpmgehmbd.html

[R07] if 判断文件
来源：http://hz.aibaodan.cn/gtqjyzsxtd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.aibaodan.cn/gtraafbqga.html

[R08] 数值比较
来源：http://hz.yangfankeji.com/gtravwubtd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.hywenlv.cn/gtalwxrjfm.html

[R09] 字符串比较
来源：http://hz.redwolf501.top/gtronljcmb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ybcxt.top/gtwcyaplvl.html

[R10] 正则匹配
来源：http://hz.yuxming.cn/gtwsgvgvjg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.sweek.top/gtvsievnqg.html

[R11] case 多分支
来源：http://hz.zhijiandao.cn/gtykgsiiua.html

case "$1" in
来源：http://hz.jianghu66.top/gtchlkdvrj.html

start) echo "启动" ;;
来源：http://hz.yuxming.cn/gtptpujqde.html

stop)  echo "停止" ;;
来源：http://hz.xuetiantiany.cn/gtlxycujzz.html

*)     echo "未知命令" ;;
来源：http://hz.cheryme.top/gtzozcgbix.html

esac
来源：http://hz.zhengqikj.top/gtinliuwge.html

[R12] for 遍历文件
来源：http://hz.yvedp.cn/gtbrrtpewf.html

for f in *.txt; do echo "$f"; done
来源：http://hz.chenjidiqi.icu/gtapjtrfnr.html

[R13] for 计数循环
来源：http://hz.zhoulong.xyz/gttqrvedbv.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xuetiantiany.cn/gttiftgxfp.html

[R14] C 风格 for
来源：http://hz.daxiang520.top/gtmtjjwfph.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cdnleiting.top/gtldbrpict.html

[R15] while 逐行读文件
来源：http://hz.jinqigfzy.top/gtksgdsist.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.daxiang520.top/gtewvddzsc.html

[R16] until 等待条件
来源：http://hz.316326.xyz/gtdyiuiaee.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.daxiang520.top/gttlyetwvc.html

[R17] 数组定义与取值
来源：http://hz.yuxming.cn/gtozowypqc.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.guannengcc.top/gtthbsxzir.html

[R18] 遍历数组
来源：http://hz.jinyuanbaomall.cn/gtpoguamxi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yj202588.top/gtlhqejejj.html

[R19] 数组长度
来源：http://hz.shanyushiyangkeji.top/gtyyzcjodb.html

echo "${#arr[@]}"
来源：http://hz.yangfankeji.com/gtubiompth.html

[R20] 关联数组（字典）
来源：http://hz.zhaomingkeji.xyz/gtqareroub.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yueranfly.top/gtoyriatex.html

[R21] 字符串长度
来源：http://hz.yanxiufei.cn/gtbkitnxbo.html

echo "${#s}"
来源：http://hz.wangdashe.top/gtudszftgk.html

[R22] 截取子串
来源：http://hz.zhongyouzk.top/gtostyujhk.html

echo "${s:0:5}"
来源：http://hz.xziqi.cn/gtsddjoonk.html

[R23] 字符串替换
来源：http://hz.jiagoushi.top/gtmgzwlhvt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yj20258888.top/gtymqulqsh.html

[R24] 大小写转换
来源：http://hz.yangfankeji.com/gtldepwvdi.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hywenlv.cn/gtqnllpdka.html

[R25] 去后缀 / 去前缀
来源：http://hz.hysaishi.cn/gtieptjhaa.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.9152youxi.cn/gtzpuifadj.html

[R26] 命令替换
来源：http://hz.yangfankeji.com/gtsakfuzia.html

now=$(date +%F); echo "$now"
来源：http://hz.cheryme.top/gtdgeefphg.html

[R27] 算术展开
来源：http://hz.bjfxy.top/gtrhqtdqrj.html

echo $((1 + 2 * 3))
来源：http://hz.yvedp.cn/gtfimxtoxs.html

[R28] 浮点运算
来源：http://hz.jinqigfzy.top/gtmwmlddts.html

echo "scale=2; 10/3" | bc
来源：http://hz.pengpengdd.cyou/gtbfuglors.html

[R29] 定义函数
来源：http://hz.iojbl.cn/gttvssowrp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yuxming.cn/gtoyjlkcqm.html

[R30] 函数返回状态码
来源：http://hz.yj202588.top/gttzbempnz.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.redwolf501.top/gtugoofspi.html

[R31] 局部变量
来源：http://hz.nanxinkj.top/gtuxyykkmf.html

f() { local x=1; echo "$x"; }
来源：http://hz.zdqjudy.top/gtorekisfi.html

[R32] 参数个数校验
来源：http://hz.cqqwz.cn/gtpxoqusdn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.chenlongwang.top/gtmymyyghf.html

[R33] 捕获错误并提示行号
来源：http://hz.yongpay.top/gtfyaafaxo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jinqigufen.top/gtezvxyboe.html

[R34] 退出时清理
来源：http://hz.xziqi.cn/gtizzsojid.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xylfe.cn/gtzypkatxa.html

[R35] 后台执行并等待
来源：http://hz.mhx1999.top/gtzzfdewni.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zycfv.cn/gtwarubrii.html

[R36] 并发执行多个任务
来源：http://hz.52xcode.cn/gtnuxwfdrf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.smart0.xyz/gthluwwnhu.html

[R37] 把输出赋给变量
来源：http://hz.52xcode.cn/gtwvfjmlor.html

files=$(ls -1)
来源：http://hz.chenlongwang.top/gtaemmcjry.html

[R38] 管道串联
来源：http://hz.xziqi.cn/gtpcqoxbck.html

cat a.txt | grep -i error | wc -l
来源：http://hz.wangdashe.top/gturjrxsna.html

[R39] 重定向标准输出与错误
来源：http://hz.ybcxt.top/gtieiutdxk.html

cmd > out.log 2>&1
来源：http://hz.zhoulong.xyz/gtrtmsaghr.html

[R40] 追加写日志
来源：http://hz.birdmap.top/gtlijngvvt.html

echo "log" >> out.log
来源：http://hz.chenjidiqi.icu/gtmthvccld.html

[R41] 丢弃输出
来源：http://hz.gotoacloud.top/gtclvomnve.html

cmd >/dev/null 2>&1
来源：http://hz.zhixingplan.top/gtdfmolwkr.html

[R42] 输入重定向
来源：http://hz.wangdashe.top/gtbytuldwy.html

wc -l < a.txt
来源：http://hz.yuxming.cn/gtpnwqisrs.html

[R43] 按名字查找文件
来源：http://hz.ydzc1.top/gtlzltslem.html

find . -name "*.log" -type f
来源：http://hz.jinqigufen.top/gttcugiurl.html

[R44] 按修改时间查找
来源：http://hz.yj20258.top/gtpznmnsgb.html

find . -mtime -7 -type f
来源：http://hz.meibo888.top/gtielowmws.html

[R45] 批量删除
来源：http://hz.jyoumei.cn/gtxpoeyyti.html

find . -name "*.tmp" -delete
来源：http://hz.c1oappe.top/gtzhsblton.html

[R46] 递归替换文件内容
来源：http://hz.hfpthk.cn/gtizkgwlcr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cqqwz.cn/gtxyrogbtm.html

[R47] sed 单行替换
来源：http://hz.jiagoushi.top/gtazythmjh.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.sufxvd.cn/gtigmcobhs.html

[R48] awk 取指定列
来源：http://hz.yuanzhike.top/gthzjjojbl.html

awk '{print $1, $3}' a.txt
来源：http://hz.yonumen.top/gtionhrpkv.html

[R49] awk 带条件
来源：http://hz.andypj.xyz/gtqbhrzslf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.havefunace.top/gtfzrhabej.html

[R50] awk 求和
来源：http://hz.cqqwz.cn/gtcfrtfdss.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.iojbl.cn/gtilsgdafi.html

[R51] 排序去重取前几
来源：http://hz.hnxiangtu.top/gtuhtdqpho.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gaohongyu789.top/gtzingfuwc.html

[R52] 统计行数
来源：http://hz.gogol.net.cn/gtzvwqjabf.html

wc -l a.txt
来源：http://hz.yuanzhike.top/gtrtccohzz.html

[R53] 查看文件头与实时尾
来源：http://hz.wangshuangyany.cn/gtvjsrwcou.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.pengpengdd.cyou/gtiyunfdum.html

[R54] 比较两个文件
来源：http://hz.sweek.top/gtjcizlnsz.html

diff a.txt b.txt
来源：http://hz.zdqjudy.top/gtchpgpxkw.html

[R55] 压缩与解压
来源：http://hz.iojbl.cn/gtscoxqdaj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.tanke756.top/gtxzlgdicu.html

[R56] 远程拷贝
来源：http://hz.hnxiangtu.top/gtsqmrngyx.html

scp file user@host:/path/
来源：http://hz.wangshuangyany.cn/gtyqqzgmtu.html

[R57] 远程执行命令
来源：http://hz.xylfe.cn/gtvihopwpk.html

ssh user@host 'uptime'
来源：http://hz.jqgufenzy.top/gtaefeyjkq.html

[R58] 下载文件
来源：http://hz.hysaishi.cn/gtmyeisedj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zdqjudy.top/gtldbxdrgw.html

[R59] 发 POST JSON
来源：http://hz.gzhubu.top/gtftygfzyf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.feifeiyinyue.top/gthauugvym.html

[R60] 只看 HTTP 状态码
来源：http://hz.ppjwa.cn/gtcapkhcxi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yonumen.top/gtwzsxfydb.html

[R61] 磁盘占用
来源：http://hz.yj20258888.top/gtdqzdaonn.html

df -h;  du -sh *
来源：http://hz.sufxvd.cn/gtooorplan.html

[R62] 找最占空间的文件
来源：http://hz.shanyushiyangkeji.top/gthgorgxac.html

du -ah . | sort -rh | head -10
来源：http://hz.cdnleiting.top/gtpshvkezp.html

[R63] 内存与进程
来源：http://hz.fengsongda.top/gtrlgwncfm.html

free -h;  ps aux | grep nginx
来源：http://hz.zhijiandao.cn/gtpwqqkipx.html

[R64] 结束进程
来源：http://hz.cheryme.top/gtvpxbrlma.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhengqikj.top/gtriuhdpad.html

[R65] 查看端口占用
来源：http://hz.daxiang520.top/gtchazfvix.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jlsjyb.cn/gttsvfhnfz.html

[R66] 定时任务
来源：http://hz.andypj.xyz/gtusfeuogh.html

crontab -e;  crontab -l
来源：http://hz.jinghuilouyu.cn/gtpavbgkky.html

[R67] 生成随机十六进制串
来源：http://hz.havefunace.top/gtgprwhzln.html

openssl rand -hex 16
来源：http://hz.zhiwuduotai.top/gtxjfbuikv.html

[R68] 计算文件校验值
来源：http://hz.bjfxy.top/gtleczwwya.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.gzhubu.top/gtqrsjvgzs.html

[R69] 生成随机密码
来源：http://hz.birdmap.top/gtttmikvfc.html

head -c 16 /dev/urandom | base64
来源：http://hz.chenzaomai.com/gtnfpuhtet.html

[R70] 时间戳与互转
来源：http://hz.hywenlv.cn/gtknypqpro.html

date +%s;  date -d @1700000000
来源：http://hz.sweek.top/gtytuygbum.html

[R71] 日期格式化
来源：http://hz.9152youxi.cn/gtqvtqbrgz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hywenlv.cn/gtngntmccx.html

[R72] 等待端口就绪
来源：http://hz.chenlongwang.top/gtfvhqvijw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yvedp.cn/gtvnydcjov.html

[R73] 分割大日志
来源：http://hz.redwolf501.top/gtvyizsnep.html

split -l 1000 big.log part_
来源：http://hz.yj202588.top/gtfgdzygzt.html

[R74] 批量重命名
来源：http://hz.sufxvd.cn/gtjtactiko.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xuanzx.com/gtkjhdxpdy.html

[R75] 导出环境变量
来源：http://hz.shanyushiyangtech.top/gtwaxwhyvz.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jinqigfzy.top/gtunoykbee.html

[R76] 使用临时文件
来源：http://hz.hfpthk.cn/gtzneyodbs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jianghu66.top/gtwhvpngxz.html

[R77] 读取用户输入
来源：http://hz.nwbrower.top/gtkvuwobjy.html

read -rp "请输入: " ans
来源：http://hz.meibo888.top/gtgnrieygy.html

[R78] 交互式菜单
来源：http://hz.cheryme.top/gtyntzwbef.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhixingplan.top/gtbvvmmton.html

[R79] 解析命令行选项
来源：http://hz.daria6918.cn/gthzutvdki.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.gogol.net.cn/gtiyefnuob.html

[R80] 查看脚本执行耗时
来源：http://hz.cashguo.top/gthgtvmdcj.html

time ./run.sh
来源：http://hz.shuidangran.top/gtvbovhrkr.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtesgrtogo.html

S. C / C++ 专题
来源：http://hz.ehwqpu.com/gtemzcegot.html

================================================================================
来源：http://hz.tian-w.cn/gtnznngqlw.html

[S01] C：Hello World
来源：http://hz.yueranfly.top/gtabohigty.html

#include <stdio.h>
来源：http://hz.nanxinkj.top/gtqrvvnhtk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xziqi.cn/gtezzwxqne.html

[S02] C：变量与格式化输出
来源：http://hz.dashuyun.cn/gtyjicwqzr.html

int a = 10; printf("%d\n", a);
来源：http://hz.hongshengwenyu.top/gtqlelcujt.html

[S03] C：读入整数
来源：http://hz.nanxinkj.top/gtjslbprze.html

int x; scanf("%d", &x);
来源：http://hz.haohaochexian.top/gttvdysntv.html

[S04] C：字符串复制
来源：http://hz.ydjk.org.cn/gtfqoyyugk.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.wangshuangyany.cn/gtkykdhblw.html

[S05] C：字符串长度
来源：http://hz.gotoacloud.top/gtejypdvll.html

strlen(s)
来源：http://hz.ywan-chungtsiang.top/gtqngzlqxg.html

[S06] C：字符串比较
来源：http://hz.jqgufenzy.top/gtdurhoxer.html

strcmp(a, b) == 0
来源：http://hz.shangyingyoupin.top/gturpuxxez.html

[S07] C：数组遍历求和
来源：http://hz.sufxvd.cn/gtkdaitmnp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.redwolf501.top/gtllroravo.html

[S08] C：动态内存分配与释放
来源：http://hz.andypj.xyz/gtkodxysid.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.fzhhl.top/gtghksgrop.html

[S09] C：结构体定义与初始化
来源：http://hz.aibaodan.cn/gtztmdacvh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jinqigufen.top/gtdfkkvfxh.html

[S10] C：指针与解引用
来源：http://hz.haohaochexian.top/gtsamnnlrb.html

int *p = &a;  *p = 5;
来源：http://hz.sweek.top/gtxqogltsn.html

[S11] C：逐行读文件
来源：http://hz.jinghuilouyu.cn/gtgovocodu.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.cqqwz.cn/gtvdqyxuzr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.gzhubu.top/gtbckavaeh.html

fclose(f);
来源：http://hz.kuanghao11.cn/gtzretsjod.html

[S12] C：写文件
来源：http://hz.yongpay.top/gtvfvmixiq.html


<!-- 参考信息 -->