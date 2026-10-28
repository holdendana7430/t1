代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://hz.xziqi.cn/gtovdowyph.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jyoumei.cn/gtpexcfvmy.html

[Q39] 自连接（查上下级）
来源：http://hz.pengpengdd.cyou/gtrvxjvnge.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhixingplan.top/gtuiqibjwy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xingfuxueyuan.xyz/gtftbztrkn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hfpthk.cn/gtwwdwnjbq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jianghu66.top/gtfuhztomz.html

[Q41] 多表连接
来源：http://hz.guowangkeji.top/gtevojrvfe.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yuanzhike.top/gtjwhppjng.html

JOIN users u ON u.id = o.user_id
来源：http://hz.meibo888.top/gtiiewbhls.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yj202588.top/gtoxqnivab.html

[Q42] 连接条件附加过滤
来源：http://hz.chenlongwang.top/gtwgeamldv.html

SELECT u.name, o.amount FROM users u
来源：http://hz.tanke756.top/gtpufaxsdb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.shanyushiyangtech.top/gtzupugcjo.html

[Q43] 标量子查询
来源：http://hz.tianlin.xyz/gtbvurapdz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ydjk.org.cn/gtxddabcnk.html

[Q44] IN 子查询
来源：http://hz.shzxlz.cn/gtkntybfwh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jqgufenzy.top/gtlwfmeqbe.html

[Q45] EXISTS 判断存在
来源：http://hz.cashguo.top/gttdtmpewc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xinyue.icu/gtigvrzofu.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yvedp.cn/gtzlggsrfs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cqqwz.cn/gtspfpkbbs.html

[Q47] 与平均值比较
来源：http://hz.jinqigufen.top/gtijlgjvwm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.0kj1m.cn/gtqcvzfilk.html

[Q48] CTE 公用表表达式
来源：http://hz.ppjwa.cn/gtayeoajdq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jiagoushi.top/gtcfzgkjit.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.sxryk.cn/gtcwsmtkqz.html

[Q49] 更新单行
来源：http://hz.xinyue.icu/gtavkdwnhj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.xingfuxueyuan.xyz/gtjeecmfhg.html

[Q50] 批量更新
来源：http://hz.c1oappe.top/gtwkpqmang.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yanxiufei.cn/gtrbpkdimb.html

[Q51] 用子查询更新
来源：http://hz.c1oappe.top/gtwtofugox.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.xziqi.cn/gtmkdbbhrm.html

[Q52] 删除指定行
来源：http://hz.zdqjudy.top/gtgmtseakz.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yanxiufei.cn/gtejjoplsq.html

[Q53] 按条件删除
来源：http://hz.ybcxt.top/gtpovvkmat.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ydzc1.top/gtszuqaqej.html

[Q54] 清空表
来源：http://hz.c1oappe.top/gtntymrjzt.html

TRUNCATE TABLE logs;
来源：http://hz.gzhubu.top/gtfwoaeqim.html

[Q55] 排名（并列占位）
来源：http://hz.yangfankeji.com/gtxinaqglj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jinqigufen.top/gtrovzqozo.html

[Q56] 密集排名（并列不占位）
来源：http://hz.havefunace.top/gtnnzarlxm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yj20258888.top/gtifmxpene.html

[Q57] 行号
来源：http://hz.zhengqikj.top/gtyuwvgkvk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zdqjudy.top/gtltaxjdmb.html

[Q58] 累计求和
来源：http://hz.c1oappe.top/gtirkrctms.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zhijiandao.cn/gtyxesnnhk.html

[Q59] 分组内累计
来源：http://hz.hammf.cn/gtwbwunfmu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.shangyingyoupin.top/gtoazewvpf.html

[Q60] 取上一行 / 下一行
来源：http://hz.haohaochexian.top/gtuzvrpmmy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.wangshuangyany.cn/gtulelzfcx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yuanzhike.top/gtohuhsryj.html

[Q61] 移动平均
来源：http://hz.ybcxt.top/gtdpnbgovy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jyoumei.cn/gtksmcshjb.html

[Q62] 分组占比
来源：http://hz.sweek.top/gttnjdzbew.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.sxryk.cn/gtbxjzzzbu.html

[Q63] 开启事务
来源：http://hz.c1oappe.top/gtakyljcxm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.cheryme.top/gtgoxsskil.html

[Q64] 提交事务
来源：http://hz.yueranfly.top/gtqpfbnavf.html

COMMIT;
来源：http://hz.haohaochexian.top/gturhdfyub.html

[Q65] 回滚事务
来源：http://hz.jinghuilouyu.cn/gtjzbzbizi.html

ROLLBACK;
来源：http://hz.yongpay.top/gtsowjznrz.html

[Q66] 行锁查询
来源：http://hz.cdnleiting.top/gtubbgxbjl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hnxiangtu.top/gtobyagymh.html

[Q67] 设置隔离级别
来源：http://hz.wangdashe.top/gtgfgclqnv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.wangdashe.top/gtudffcjrn.html

[Q68] 保存点
来源：http://hz.shanyushiyangtech.top/gtxvorcrfg.html

SAVEPOINT sp1;
来源：http://hz.jinghuilouyu.cn/gtswsdsgsu.html

ROLLBACK TO sp1;
来源：http://hz.yueranfly.top/gtfpdqroml.html

[Q69] 查看执行计划
来源：http://hz.zhixingplan.top/gtnnemymkt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.svipenyu.cn/gtbxpsbeqt.html

[Q70] 更新统计信息
来源：http://hz.zhaomingkeji.xyz/gtslbygbyd.html

ANALYZE TABLE users;
来源：http://hz.jiagoushi.top/gtjywmdzzp.html

[Q71] 查看建表语句
来源：http://hz.chenlongwang.top/gtneduexwb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.sysykeji.top/gtgsfprmwn.html

[Q72] 查看索引
来源：http://hz.hnxiangtu.top/gtlcghgpad.html

SHOW INDEX FROM users;
来源：http://hz.fzhhl.top/gtbtkfngph.html

[Q73] 查看表状态
来源：http://hz.andypj.xyz/gttkitihzd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.svipenyu.cn/gtcmugldzl.html

[Q74] 强制使用索引
来源：http://hz.9152youxi.cn/gtnbsvbess.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.c1oappe.top/gthbfkldwu.html

[Q75] 日期格式化
来源：http://hz.daria6918.cn/gtcdmhybwj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhoulong.xyz/gtldappxzl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yvedp.cn/gtqngrnlbc.html

[Q76] 按天统计
来源：http://hz.316326.xyz/gtqpjbiofi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.cdnleiting.top/gttuflznuu.html

[Q77] 时间加减
来源：http://hz.ybcxt.top/gtogmjxjre.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.daria6918.cn/gtqxultzsb.html

[Q78] 当前时间
来源：http://hz.yuxming.cn/gtmfbyymll.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.shanyushiyangtech.top/gtqjojetjy.html

[Q79] 字符串拼接
来源：http://hz.chenzaomai.com/gtyqmskvat.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.0kj1m.cn/gtbpgsjgtz.html

[Q80] 字符串截取
来源：http://hz.cheryme.top/gtagtudqyh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.dianchejie.cn/gtdgqptcye.html

[Q81] 字符串替换
来源：http://hz.yvedp.cn/gttvjjkazi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yuxming.cn/gttouyyglp.html

[Q82] 字符长度与字节长度
来源：http://hz.jlsjyb.cn/gtuxomuiei.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.pengpengdd.cyou/gtxpqeixjn.html

[Q83] 大小写转换
来源：http://hz.mhx1999.top/gtpbkfhtvf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.tianlin.xyz/gtfetsmxaw.html

[Q84] 去除首尾空格
来源：http://hz.jinyuanbaomall.cn/gtknwomqat.html

SELECT TRIM(name) FROM users;
来源：http://hz.ppjwa.cn/gtxkudoohn.html

[Q85] 数值取整
来源：http://hz.yuxming.cn/gtteurptgy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.hammf.cn/gtvspqkgxe.html

[Q86] 读取 JSON 字段
来源：http://hz.meibo888.top/gtuffjjdbl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yj20258888.top/gttwgrxoaq.html

[Q87] JSON 字段做条件
来源：http://hz.sweek.top/gtiuzfomyq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ywan-chungtsiang.top/gtfeaixxkb.html

[Q88] 行转列（条件聚合）
来源：http://hz.hnxiangtu.top/gtqacfyowa.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhengqikj.top/gtijlabmzk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hnxiangtu.top/gtlmjafvyp.html

[Q89] 判断表是否存在
来源：http://hz.jlsjyb.cn/gtnqdeduel.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ehwqpu.com/gtnbtuhcxc.html

[Q90] 生成序号列
来源：http://hz.xziqi.cn/gtyfnnqqpz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.fengsongda.top/gtwaaezyig.html

================================================================================
来源：http://hz.ppjwa.cn/gtqzdpzdtj.html

R. Bash 专题
来源：http://hz.xinyue.icu/gtemyivvoo.html

================================================================================
来源：http://hz.yuxming.cn/gtxrcjbbgi.html

[R01] shebang 与严格模式
来源：http://hz.andypj.xyz/gtzryyecvi.html

#!/usr/bin/env bash
来源：http://hz.ppjwa.cn/gtemlkianb.html

set -euo pipefail
来源：http://hz.ydjk.org.cn/gtamxpsjgb.html

[R02] 变量赋值与使用
来源：http://hz.jinqigufen.top/gthecxavbt.html

name="Tom"; echo "$name"
来源：http://hz.dashuyun.cn/gtzdvfqnvg.html

[R03] 只读变量
来源：http://hz.jinghuilouyu.cn/gtcaauwvpf.html

readonly PI=3.14
来源：http://hz.snrcjt.cn/gtcckgkqrp.html

[R04] 位置参数
来源：http://hz.hywenlv.cn/gtbuixlopi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhaomingkeji.xyz/gtmatefmdi.html

[R05] 参数默认值
来源：http://hz.svipenyu.cn/gtlxbqvzta.html

name="${1:-default}"
来源：http://hz.haohaochexian.top/gtvazchkns.html

[R06] 判断命令是否存在
来源：http://hz.jinghuilouyu.cn/gtmsmssvfb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yanxiufei.cn/gtjrstxqcg.html

[R07] if 判断文件
来源：http://hz.ppjwa.cn/gtnvbiutsl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yj202588.top/gtaxpxxudx.html

[R08] 数值比较
来源：http://hz.yongpay.top/gtznzbeprn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.svipenyu.cn/gtgyigxykr.html

[R09] 字符串比较
来源：http://hz.redwolf501.top/gtdwtqpecg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ybcxt.top/gtzwhhyazc.html

[R10] 正则匹配
来源：http://hz.dianchejie.cn/gtpdsowmli.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.kuanghao11.cn/gtvvvwccyw.html

[R11] case 多分支
来源：http://hz.jinyuanbaomall.cn/gtvgritrxr.html

case "$1" in
来源：http://hz.jqgufenzy.top/gtofjswrzc.html

start) echo "启动" ;;
来源：http://hz.gotoacloud.top/gtjawdzzjg.html

stop)  echo "停止" ;;
来源：http://hz.316326.xyz/gttxeuvlik.html

*)     echo "未知命令" ;;
来源：http://hz.chenjidiqi.icu/gtxhieojcb.html

esac
来源：http://hz.bjfxy.top/gtapmjyylm.html

[R12] for 遍历文件
来源：http://hz.shuidangran.top/gtycyppusg.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yangfankeji.com/gtzsictvfn.html

[R13] for 计数循环
来源：http://hz.chenlongwang.top/gtytfffqsi.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.havefunace.top/gtiqksfync.html

[R14] C 风格 for
来源：http://hz.jqgufenzy.top/gtgujjfhyq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xinyue.icu/gtdshslwxl.html

[R15] while 逐行读文件
来源：http://hz.hysaishi.cn/gtctbfpmpz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.chenlongwang.top/gtoelnfmeu.html

[R16] until 等待条件
来源：http://hz.hfpthk.cn/gtcnoysydq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.nwbrower.top/gtopmuqlsf.html

[R17] 数组定义与取值
来源：http://hz.jqgfzy.top/gtvdmuyutr.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zycfv.cn/gtxcmnliyi.html

[R18] 遍历数组
来源：http://hz.yangfankeji.com/gtrhkjcakh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.haohaochexian.top/gtzgrmfhsl.html

[R19] 数组长度
来源：http://hz.nanxinkj.top/gtmexjjklk.html

echo "${#arr[@]}"
来源：http://hz.52xcode.cn/gtaubfhkxq.html

[R20] 关联数组（字典）
来源：http://hz.shangyingyoupin.top/gtcbbsyjpt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.nanxuanxn.top/gtmjgaypqx.html

[R21] 字符串长度
来源：http://hz.andypj.xyz/gtklwgmqlq.html

echo "${#s}"
来源：http://hz.yuanzhike.top/gtdwrxylah.html

[R22] 截取子串
来源：http://hz.daria6918.cn/gttjjmdayg.html

echo "${s:0:5}"
来源：http://hz.guannengcc.top/gtzkpdjuil.html

[R23] 字符串替换
来源：http://hz.gotoacloud.top/gtxuurwsay.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xuanzx.com/gtbagdremb.html

[R24] 大小写转换
来源：http://hz.jinqigufen.top/gtegwnswgs.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yvedp.cn/gtkpwbsczl.html

[R25] 去后缀 / 去前缀
来源：http://hz.fengsongda.top/gtpjgvaxnj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.sweek.top/gthdldcbxj.html

[R26] 命令替换
来源：http://hz.shuidangran.top/gtbqanpwhu.html

now=$(date +%F); echo "$now"
来源：http://hz.dashuyun.cn/gtrverogap.html

[R27] 算术展开
来源：http://hz.quarkkingdee.top/gtlurtclvl.html

echo $((1 + 2 * 3))
来源：http://hz.svipenyu.cn/gtojlegrgh.html

[R28] 浮点运算
来源：http://hz.bjfxy.top/gtofqjuzmt.html

echo "scale=2; 10/3" | bc
来源：http://hz.daria6918.cn/gtaervbtsg.html

[R29] 定义函数
来源：http://hz.nwbrower.top/gtxqtxifkn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.daria6918.cn/gtktdbyhcu.html

[R30] 函数返回状态码
来源：http://hz.chenzaomai.com/gtbsecejnd.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.aibaodan.cn/gtmriezyxz.html

[R31] 局部变量
来源：http://hz.hammf.cn/gthcbcvdzi.html

f() { local x=1; echo "$x"; }
来源：http://hz.shuidangran.top/gtplkmpfki.html

[R32] 参数个数校验
来源：http://hz.zhengqikj.top/gtzagwdinj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.shanyushiyangtech.top/gtmtqftiau.html

[R33] 捕获错误并提示行号
来源：http://hz.jiagoushi.top/gtounsncea.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhoulong.xyz/gtyznnauko.html

[R34] 退出时清理
来源：http://hz.0kj1m.cn/gthmmltyox.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj20258.top/gtlnbkxljj.html

[R35] 后台执行并等待
来源：http://hz.yanxiufei.cn/gtyzzmjylu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xinyue.icu/gtcxxjqfgu.html

[R36] 并发执行多个任务
来源：http://hz.andypj.xyz/gtgsetjnds.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.redwolf501.top/gtskuowwsw.html

[R37] 把输出赋给变量
来源：http://hz.zhixingplan.top/gtfenxshau.html

files=$(ls -1)
来源：http://hz.haohaochexian.top/gtiqsmqiwc.html

[R38] 管道串联
来源：http://hz.jyoumei.cn/gtiebrgpjx.html

cat a.txt | grep -i error | wc -l
来源：http://hz.c1oappe.top/gthscuthvq.html

[R39] 重定向标准输出与错误
来源：http://hz.hfpthk.cn/gtayxsbjwd.html

cmd > out.log 2>&1
来源：http://hz.shanyushiyangkeji.top/gtdkrkucyp.html

[R40] 追加写日志
来源：http://hz.yanxiufei.cn/gtumqvzavx.html

echo "log" >> out.log
来源：http://hz.cucudq.cn/gtnbtwghbb.html

[R41] 丢弃输出
来源：http://hz.xuanzx.com/gtzhuflpbj.html

cmd >/dev/null 2>&1
来源：http://hz.jqgfzy.top/gtfivshomt.html

[R42] 输入重定向
来源：http://hz.haohaochexian.top/gtwfeidimz.html

wc -l < a.txt
来源：http://hz.yanxiufei.cn/gtdpokmpta.html

[R43] 按名字查找文件
来源：http://hz.cqqwz.cn/gtjckyblno.html

find . -name "*.log" -type f
来源：http://hz.shanyushiyangkeji.top/gtzseqgses.html

[R44] 按修改时间查找
来源：http://hz.meibo888.top/gtztethnsj.html

find . -mtime -7 -type f
来源：http://hz.iojbl.cn/gttfngndon.html

[R45] 批量删除
来源：http://hz.cqqwz.cn/gtftqdwnjl.html

find . -name "*.tmp" -delete
来源：http://hz.gogol.net.cn/gtdsmybisy.html

[R46] 递归替换文件内容
来源：http://hz.wangshuangyany.cn/gtevazyrjy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.0kj1m.cn/gtpgfawywv.html

[R47] sed 单行替换
来源：http://hz.hysaishi.cn/gtvdacvqjm.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.bjfxy.top/gtceleuevn.html

[R48] awk 取指定列
来源：http://hz.zhaomingkeji.xyz/gtgboqtlgm.html

awk '{print $1, $3}' a.txt
来源：http://hz.dianchejie.cn/gtdukctviz.html

[R49] awk 带条件
来源：http://hz.chenjidiqi.icu/gtatpbpelq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.redwolf501.top/gtiegmchks.html

[R50] awk 求和
来源：http://hz.0kj1m.cn/gtnesdeskx.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hfpthk.cn/gtgruiahqb.html

[R51] 排序去重取前几
来源：http://hz.smart0.xyz/gtdtqcdzvt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.dashuyun.cn/gtgxrvcibp.html

[R52] 统计行数
来源：http://hz.tanke756.top/gtlzakveke.html

wc -l a.txt
来源：http://hz.ivvv.top/gtrxivdgzw.html

[R53] 查看文件头与实时尾
来源：http://hz.xinyue.icu/gtpyfybewq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ehwqpu.com/gtbttptiab.html

[R54] 比较两个文件
来源：http://hz.ydjk.org.cn/gtkzwfkoqm.html

diff a.txt b.txt
来源：http://hz.xziqi.cn/gthaedntvo.html

[R55] 压缩与解压
来源：http://hz.xinyue.icu/gtxzpsggqc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.mhx1999.top/gtkiucaipy.html

[R56] 远程拷贝
来源：http://hz.tanke756.top/gtksmmazza.html

scp file user@host:/path/
来源：http://hz.chenzaomai.com/gtympsvivx.html

[R57] 远程执行命令
来源：http://hz.zhijiandao.cn/gtbzaxkmzn.html

ssh user@host 'uptime'
来源：http://hz.aibaodan.cn/gtgxrguzji.html

[R58] 下载文件
来源：http://hz.hnqzz.top/gtpdarjyft.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gzhubu.top/gtdejidiea.html

[R59] 发 POST JSON
来源：http://hz.c1oappe.top/gtvxcuteal.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jlsjyb.cn/gtjhpbjqef.html

[R60] 只看 HTTP 状态码
来源：http://hz.yuanzhike.top/gtxgbyfuvr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.fzhhl.top/gtebzhhwav.html

[R61] 磁盘占用
来源：http://hz.chenjidiqi.icu/gtrsjxtffn.html

df -h;  du -sh *
来源：http://hz.yj20258.top/gtgkdshpnl.html

[R62] 找最占空间的文件
来源：http://hz.shzxlz.cn/gtzvjwcdpe.html

du -ah . | sort -rh | head -10
来源：http://hz.dashuyun.cn/gtonyzmepc.html

[R63] 内存与进程
来源：http://hz.fengsongda.top/gtnxxgcqja.html

free -h;  ps aux | grep nginx
来源：http://hz.andypj.xyz/gtuyspopza.html

[R64] 结束进程
来源：http://hz.andypj.xyz/gtvqfuaatt.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hywenlv.cn/gtxokbjxoj.html

[R65] 查看端口占用
来源：http://hz.zdqjudy.top/gtcaofmzah.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.gaohongyu789.top/gtrlgtnslo.html

[R66] 定时任务
来源：http://hz.cucudq.cn/gtzzqpapbx.html

crontab -e;  crontab -l
来源：http://hz.xinyue.icu/gtyhnjjyov.html

[R67] 生成随机十六进制串
来源：http://hz.ppjwa.cn/gteveflydv.html

openssl rand -hex 16
来源：http://hz.316326.xyz/gtfsffccit.html

[R68] 计算文件校验值
来源：http://hz.tian-w.cn/gtdoyuqsgh.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.quarkkingdee.top/gtvrcbxiuo.html

[R69] 生成随机密码
来源：http://hz.snrcjt.cn/gtbmfnygjx.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhaomingkeji.xyz/gtevgtlnye.html

[R70] 时间戳与互转
来源：http://hz.sweek.top/gtfpkfnhxe.html

date +%s;  date -d @1700000000
来源：http://hz.zhoulong.xyz/gtjzzazuvx.html

[R71] 日期格式化
来源：http://hz.ehwqpu.com/gtrgvoesna.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cqqwz.cn/gtfxsslhyq.html

[R72] 等待端口就绪
来源：http://hz.52xcode.cn/gtikdsyzmi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jlsjyb.cn/gtcyqrjwge.html

[R73] 分割大日志
来源：http://hz.xziqi.cn/gtwmufmzpr.html

split -l 1000 big.log part_
来源：http://hz.smart0.xyz/gtccurbimv.html

[R74] 批量重命名
来源：http://hz.ppjwa.cn/gtjqfvsjfc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jiagoushi.top/gtwhybfboe.html

[R75] 导出环境变量
来源：http://hz.ivvv.top/gtjomcrkzd.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.gzhubu.top/gtvhmefpkl.html

[R76] 使用临时文件
来源：http://hz.yvedp.cn/gteyguhtwa.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hysaishi.cn/gtnhncruvh.html

[R77] 读取用户输入
来源：http://hz.chenzaomai.com/gtoxmwmexr.html

read -rp "请输入: " ans
来源：http://hz.cdnleiting.top/gtmhqouwpg.html

[R78] 交互式菜单
来源：http://hz.cucudq.cn/gtojpaedsu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.sysykeji.top/gteavksoge.html

[R79] 解析命令行选项
来源：http://hz.ivvv.top/gttwcjcwdu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.chenlongwang.top/gtitzlhxrf.html

[R80] 查看脚本执行耗时
来源：http://hz.jqgufenzy.top/gtghtflvla.html

time ./run.sh
来源：http://hz.smart0.xyz/gtfnrkelbw.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtrgsqnvgr.html

S. C / C++ 专题
来源：http://hz.snrcjt.cn/gtddzkgyto.html

================================================================================
来源：http://hz.aizwys.cn/gtasbnncyi.html

[S01] C：Hello World
来源：http://hz.jinghuilouyu.cn/gtkivutsva.html

#include <stdio.h>
来源：http://hz.meibo888.top/gthsejosdr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jinqigufen.top/gtxzscgosw.html

[S02] C：变量与格式化输出
来源：http://hz.jqgufenzy.top/gtlfbzgrow.html

int a = 10; printf("%d\n", a);
来源：http://hz.jqgufenzy.top/gtghsqiymc.html

[S03] C：读入整数
来源：http://hz.mhx1999.top/gtreblqrqs.html

int x; scanf("%d", &x);
来源：http://hz.cucudq.cn/gtlxhfjpge.html

[S04] C：字符串复制
来源：http://hz.chenlongwang.top/gtddneeyfi.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.chenzaomai.com/gtcdsnmoxp.html

[S05] C：字符串长度
来源：http://hz.smart0.xyz/gtgrtfzbug.html

strlen(s)
来源：http://hz.yvedp.cn/gtgdyleknx.html

[S06] C：字符串比较
来源：http://hz.chenzaomai.com/gthhszlpnx.html

strcmp(a, b) == 0
来源：http://hz.feifeiyinyue.top/gtaprwdagj.html

[S07] C：数组遍历求和
来源：http://hz.cashguo.top/gtkkqeacgb.html


<!-- 参考信息 -->