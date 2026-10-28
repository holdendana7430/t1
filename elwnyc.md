代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ivvv.top/gtugwpqiss.html

) t WHERE rn = 1;
来源：http://hz.sysykeji.top/gtdksjmgkk.html

[Q35] 内连接
来源：http://hz.fengsongda.top/gtcowytyoq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhaomingkeji.xyz/gtbhkdkahw.html

[Q36] 左连接
来源：http://hz.sysykeji.top/gtghnuinjr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.guowangkeji.top/gtznepsvdr.html

[Q37] 右连接
来源：http://hz.gotoacloud.top/gtlqkxzxna.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.meibo888.top/gtklvrhfpu.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.gotoacloud.top/gtukaioccs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.gogol.net.cn/gtsyiatgmr.html

[Q39] 自连接（查上下级）
来源：http://hz.pengpengdd.cyou/gtzpcascol.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhijiandao.cn/gtoelxxmun.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ywan-chungtsiang.top/gtrhpbxera.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.chenjidiqi.icu/gtbqgfjkhr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.tian-w.cn/gtnxewxpjx.html

[Q41] 多表连接
来源：http://hz.xuetiantiany.cn/gtmpffyctd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yj202588.top/gtotkgodhe.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hysaishi.cn/gtwkadgybz.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jiagoushi.top/gtmdifkvxo.html

[Q42] 连接条件附加过滤
来源：http://hz.jinghuilouyu.cn/gtkfzvfurc.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hnqzz.top/gtscolajbh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.mhx1999.top/gtejvyztxt.html

[Q43] 标量子查询
来源：http://hz.jinghuilouyu.cn/gtwjgnfyaf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.52xcode.cn/gtpqjdpihd.html

[Q44] IN 子查询
来源：http://hz.chenzaomai.com/gtrqnvxelk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.cheryme.top/gtsjzgbkkx.html

[Q45] EXISTS 判断存在
来源：http://hz.sysykeji.top/gtbuewzikh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gogol.net.cn/gtztpvtqum.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.dianchejie.cn/gtjrdprbyy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.chenzaomai.com/gtorespdyx.html

[Q47] 与平均值比较
来源：http://hz.yonumen.top/gtulhmvdqz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.tianlin.xyz/gthiilynif.html

[Q48] CTE 公用表表达式
来源：http://hz.sxryk.cn/gtwszwiouv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.tianlin.xyz/gtrwvxaqtx.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.0kj1m.cn/gtsvybqaiy.html

[Q49] 更新单行
来源：http://hz.jinqigufen.top/gtstnxoado.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hongshengwenyu.top/gtfkwyzaob.html

[Q50] 批量更新
来源：http://hz.wangshuangyany.cn/gtcwhbhklm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.bjfxy.top/gtbpfufvye.html

[Q51] 用子查询更新
来源：http://hz.havefunace.top/gthmjneiky.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.bjfxy.top/gtqwdektte.html

[Q52] 删除指定行
来源：http://hz.yanxiufei.cn/gtwnrampao.html

DELETE FROM users WHERE id = 10;
来源：http://hz.cashguo.top/gtfeefkqgy.html

[Q53] 按条件删除
来源：http://hz.0kj1m.cn/gtwkxozoxm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yanxiufei.cn/gtdbpjswyi.html

[Q54] 清空表
来源：http://hz.jinqigfzy.top/gtrropwduu.html

TRUNCATE TABLE logs;
来源：http://hz.zdqjudy.top/gtnbvoqesq.html

[Q55] 排名（并列占位）
来源：http://hz.shanyushiyangtech.top/gtpobvzfja.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ehwqpu.com/gtyfyaqxru.html

[Q56] 密集排名（并列不占位）
来源：http://hz.nanxinkj.top/gtvqpiszbk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ehwqpu.com/gtxxitknku.html

[Q57] 行号
来源：http://hz.cashguo.top/gtjnfgvazf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.tianlin.xyz/gtknsyexor.html

[Q58] 累计求和
来源：http://hz.shanyushiyangtech.top/gtdghmksxy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jinqigfzy.top/gthphcxhgc.html

[Q59] 分组内累计
来源：http://hz.gaohongyu789.top/gtlqeupmac.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.shanyushiyangtech.top/gtbbymfbvx.html

[Q60] 取上一行 / 下一行
来源：http://hz.ppjwa.cn/gtkphivftd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.tanke756.top/gtymgvkauz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.cqqwz.cn/gtwisyudbl.html

[Q61] 移动平均
来源：http://hz.zhengqikj.top/gtspqushqb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.pycfn.com/gtfgzdiojg.html

[Q62] 分组占比
来源：http://hz.jlsjyb.cn/gtrheodwuu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ydjk.org.cn/gtqczkvplj.html

[Q63] 开启事务
来源：http://hz.bjfxy.top/gtorgwqikm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.nanxinkj.top/gtvtsmmfkp.html

[Q64] 提交事务
来源：http://hz.yj20258888.top/gttolseblp.html

COMMIT;
来源：http://hz.yueranfly.top/gtzvmjtcjb.html

[Q65] 回滚事务
来源：http://hz.aibaodan.cn/gtnbslruac.html

ROLLBACK;
来源：http://hz.sufxvd.cn/gtptfdpeic.html

[Q66] 行锁查询
来源：http://hz.quarkkingdee.top/gtonhyqxpk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.feifeiyinyue.top/gtcqbfdfxs.html

[Q67] 设置隔离级别
来源：http://hz.0kj1m.cn/gtqxwzryio.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.daria6918.cn/gtxgtyvpwy.html

[Q68] 保存点
来源：http://hz.ydjk.org.cn/gtoswsneap.html

SAVEPOINT sp1;
来源：http://hz.yangfankeji.com/gtpurwapyq.html

ROLLBACK TO sp1;
来源：http://hz.shanyushiyangtech.top/gtxzdxhzsi.html

[Q69] 查看执行计划
来源：http://hz.ppjwa.cn/gtrnpsatvb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.gaohongyu789.top/gthfhsiilz.html

[Q70] 更新统计信息
来源：http://hz.zycfv.cn/gtizfyuoxl.html

ANALYZE TABLE users;
来源：http://hz.mhx1999.top/gtrlshrkqt.html

[Q71] 查看建表语句
来源：http://hz.jiagoushi.top/gtvmhztsae.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.tanke756.top/gtenezkuki.html

[Q72] 查看索引
来源：http://hz.ywan-chungtsiang.top/gtppzhuovx.html

SHOW INDEX FROM users;
来源：http://hz.aizwys.cn/gtylyjivsz.html

[Q73] 查看表状态
来源：http://hz.jqgfzy.top/gtvpkqfmke.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yvedp.cn/gtojqaldjk.html

[Q74] 强制使用索引
来源：http://hz.sufxvd.cn/gtcbqbflic.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.daria6918.cn/gtkyhnaijx.html

[Q75] 日期格式化
来源：http://hz.cucudq.cn/gtmfqekhmg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.andypj.xyz/gtgcyddgyd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.kuanghao11.cn/gtudzdsegd.html

[Q76] 按天统计
来源：http://hz.shanyushiyangkeji.top/gtmibszihh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.fengsongda.top/gtnwbphpwq.html

[Q77] 时间加减
来源：http://hz.hongshengwenyu.top/gtpemzgxmn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.tianlin.xyz/gtexqlwtgd.html

[Q78] 当前时间
来源：http://hz.shuidangran.top/gtsfyyysvm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yj202588.top/gtebnoihsf.html

[Q79] 字符串拼接
来源：http://hz.shzxlz.cn/gtnntxrgim.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jinqigfzy.top/gtvdetvbvt.html

[Q80] 字符串截取
来源：http://hz.iojbl.cn/gtyqjuwgka.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.sufxvd.cn/gtbbgdsxtc.html

[Q81] 字符串替换
来源：http://hz.9152youxi.cn/gtrrlcbiog.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.vqdsnc.cn/gtpwxypjqr.html

[Q82] 字符长度与字节长度
来源：http://hz.aibaodan.cn/gtynkodupe.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.sweek.top/gtlffjkoms.html

[Q83] 大小写转换
来源：http://hz.zhongyouzk.top/gtjosrskwu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.cdnleiting.top/gttheuuxdi.html

[Q84] 去除首尾空格
来源：http://hz.tanke756.top/gtjtiyxbsm.html

SELECT TRIM(name) FROM users;
来源：http://hz.zdqjudy.top/gtruuwibwu.html

[Q85] 数值取整
来源：http://hz.yuxming.cn/gtxsysajfr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yonumen.top/gtwficfewx.html

[Q86] 读取 JSON 字段
来源：http://hz.pengpengdd.cyou/gtmxjgyzgc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jyoumei.cn/gtoambjirs.html

[Q87] JSON 字段做条件
来源：http://hz.shangyingyoupin.top/gtltwhgwaj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yj20258.top/gtygabykqb.html

[Q88] 行转列（条件聚合）
来源：http://hz.ybcxt.top/gtgvqfcptm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.gotoacloud.top/gtmilllnxz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jqgfzy.top/gtzanowvlv.html

[Q89] 判断表是否存在
来源：http://hz.yj20258.top/gtcjsfhqnx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.sufxvd.cn/gtbttxxziq.html

[Q90] 生成序号列
来源：http://hz.ywan-chungtsiang.top/gtkslcombo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yuxming.cn/gtvnifqoce.html

================================================================================
来源：http://hz.hammf.cn/gtitoqveya.html

R. Bash 专题
来源：http://hz.ydjk.org.cn/gtozxgnkjf.html

================================================================================
来源：http://hz.pycfn.com/gtojsjyqqs.html

[R01] shebang 与严格模式
来源：http://hz.zhiwuduotai.top/gtnlmhytso.html

#!/usr/bin/env bash
来源：http://hz.ywan-chungtsiang.top/gtmlnmpdfj.html

set -euo pipefail
来源：http://hz.cheryme.top/gtguxfgdgr.html

[R02] 变量赋值与使用
来源：http://hz.yuxming.cn/gtzrvponxu.html

name="Tom"; echo "$name"
来源：http://hz.xinyue.icu/gtrnylbchq.html

[R03] 只读变量
来源：http://hz.chenlongwang.top/gtqxxrmxwb.html

readonly PI=3.14
来源：http://hz.haohaochexian.top/gtqgpgfkmb.html

[R04] 位置参数
来源：http://hz.daxiang520.top/gtexqemyks.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hongshengwenyu.top/gtkokbcbvl.html

[R05] 参数默认值
来源：http://hz.jinghuilouyu.cn/gtyysyfkjm.html

name="${1:-default}"
来源：http://hz.0kj1m.cn/gtpgmdjjca.html

[R06] 判断命令是否存在
来源：http://hz.yj20258888.top/gtvskbzugn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xingfuxueyuan.xyz/gtcgiwhaqd.html

[R07] if 判断文件
来源：http://hz.aibaodan.cn/gtkkuytpvp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ywan-chungtsiang.top/gteaqnbafy.html

[R08] 数值比较
来源：http://hz.9152youxi.cn/gtssovunnv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jiagoushi.top/gtkeeekiow.html

[R09] 字符串比较
来源：http://hz.xinyue.icu/gtpoafznbm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hfpthk.cn/gtuywjetpy.html

[R10] 正则匹配
来源：http://hz.cheryme.top/gtqcepwpei.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.kuanghao11.cn/gtwhfuyvkz.html

[R11] case 多分支
来源：http://hz.tianlin.xyz/gtaoyyrnbg.html

case "$1" in
来源：http://hz.svipenyu.cn/gtkrvsbxac.html

start) echo "启动" ;;
来源：http://hz.hnqzz.top/gtzabjpoct.html

stop)  echo "停止" ;;
来源：http://hz.svipenyu.cn/gtokuzrqpv.html

*)     echo "未知命令" ;;
来源：http://hz.chenzaomai.com/gtbtxjibum.html

esac
来源：http://hz.chenzaomai.com/gtoipruqpf.html

[R12] for 遍历文件
来源：http://hz.shuidangran.top/gtxatgmsch.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ivvv.top/gtjsqdncxm.html

[R13] for 计数循环
来源：http://hz.pycfn.com/gtiigiqbta.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.gotoacloud.top/gthrfsfqvz.html

[R14] C 风格 for
来源：http://hz.52xcode.cn/gtlkmqglpp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yj20258888.top/gtostoqvjr.html

[R15] while 逐行读文件
来源：http://hz.zhengqikj.top/gtpcpyyyme.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hywenlv.cn/gtvlrewjps.html

[R16] until 等待条件
来源：http://hz.jyoumei.cn/gtsnxqpqnc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhaomingkeji.xyz/gthxszzfot.html

[R17] 数组定义与取值
来源：http://hz.kuanghao11.cn/gtzlbexftc.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhixingplan.top/gtmwujqlfb.html

[R18] 遍历数组
来源：http://hz.aibaodan.cn/gtgmvextnj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xylfe.cn/gtednmlkvj.html

[R19] 数组长度
来源：http://hz.cucudq.cn/gtrplagmbo.html

echo "${#arr[@]}"
来源：http://hz.yvedp.cn/gtsujanihe.html

[R20] 关联数组（字典）
来源：http://hz.zhoulong.xyz/gtysqplezg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.pengpengdd.cyou/gtyjrdjsty.html

[R21] 字符串长度
来源：http://hz.shzxlz.cn/gtsmdmldup.html

echo "${#s}"
来源：http://hz.xuetiantiany.cn/gtjnzzigno.html

[R22] 截取子串
来源：http://hz.cdnleiting.top/gtlsvkopnp.html

echo "${s:0:5}"
来源：http://hz.cashguo.top/gtwpvwntmi.html

[R23] 字符串替换
来源：http://hz.daxiang520.top/gthbjopyhp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.wangshuangyany.cn/gteuxwteow.html

[R24] 大小写转换
来源：http://hz.cucudq.cn/gttkwfsfku.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.feifeiyinyue.top/gtpvihiblx.html

[R25] 去后缀 / 去前缀
来源：http://hz.meibo888.top/gtvoirkdiv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.gaohongyu789.top/gtnksgyrvj.html

[R26] 命令替换
来源：http://hz.52xcode.cn/gtsxooslhv.html

now=$(date +%F); echo "$now"
来源：http://hz.yj20258888.top/gtnhqdapae.html

[R27] 算术展开
来源：http://hz.sxryk.cn/gtaqanawgu.html

echo $((1 + 2 * 3))
来源：http://hz.9152youxi.cn/gtxjgqbtcf.html

[R28] 浮点运算
来源：http://hz.zhongyouzk.top/gtfmzagnru.html

echo "scale=2; 10/3" | bc
来源：http://hz.jinghuilouyu.cn/gtjhpunnkl.html

[R29] 定义函数
来源：http://hz.quarkkingdee.top/gtuauduozl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yanxiufei.cn/gtdqgkvmlw.html

[R30] 函数返回状态码
来源：http://hz.daria6918.cn/gtvawkyduw.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.nwbrower.top/gtwnoxqlbt.html

[R31] 局部变量
来源：http://hz.nwbrower.top/gttmerbfxj.html

f() { local x=1; echo "$x"; }
来源：http://hz.pycfn.com/gtxfjgmpfs.html

[R32] 参数个数校验
来源：http://hz.kuanghao11.cn/gtwbfhayyw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.dashuyun.cn/gtnuiymjpx.html

[R33] 捕获错误并提示行号
来源：http://hz.jinyuanbaomall.cn/gtnbowzbgd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhongyouzk.top/gtbwrdyxtf.html

[R34] 退出时清理
来源：http://hz.cucudq.cn/gtlldorjwe.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhaomingkeji.xyz/gtutfkyrhc.html

[R35] 后台执行并等待
来源：http://hz.ybcxt.top/gtaisgfgmg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.guannengcc.top/gtazxlbozx.html

[R36] 并发执行多个任务
来源：http://hz.kuanghao11.cn/gtqyitevlu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shangyingyoupin.top/gtjmxscrdv.html

[R37] 把输出赋给变量
来源：http://hz.meibo888.top/gtgrdgxqxr.html

files=$(ls -1)
来源：http://hz.aizwys.cn/gtpqjdvhci.html

[R38] 管道串联
来源：http://hz.snrcjt.cn/gttvukhumj.html

cat a.txt | grep -i error | wc -l
来源：http://hz.shangyingyoupin.top/gtsqwzhtqn.html

[R39] 重定向标准输出与错误
来源：http://hz.hysaishi.cn/gtcgyufhfc.html

cmd > out.log 2>&1
来源：http://hz.andypj.xyz/gtxfyflqjg.html

[R40] 追加写日志
来源：http://hz.tianlin.xyz/gtcxardyqg.html

echo "log" >> out.log
来源：http://hz.ybcxt.top/gthkduurvi.html

[R41] 丢弃输出
来源：http://hz.nwbrower.top/gtpntzcgww.html

cmd >/dev/null 2>&1
来源：http://hz.meibo888.top/gtxvmulmwv.html

[R42] 输入重定向
来源：http://hz.xinyue.icu/gtpyyvufer.html

wc -l < a.txt
来源：http://hz.yuxming.cn/gtqmnbivpi.html

[R43] 按名字查找文件
来源：http://hz.zhoulong.xyz/gtgofijukl.html

find . -name "*.log" -type f
来源：http://hz.nanxinkj.top/gtiroglqkk.html

[R44] 按修改时间查找
来源：http://hz.gaohongyu789.top/gtivoynzjx.html

find . -mtime -7 -type f
来源：http://hz.ywan-chungtsiang.top/gthcreyqrh.html

[R45] 批量删除
来源：http://hz.cucudq.cn/gtfnnvwifv.html

find . -name "*.tmp" -delete
来源：http://hz.tian-w.cn/gtdmcfvvkd.html

[R46] 递归替换文件内容
来源：http://hz.cheryme.top/gtffvreudb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jinqigfzy.top/gtanjmbnto.html

[R47] sed 单行替换
来源：http://hz.sxryk.cn/gtvfcxwghn.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xylfe.cn/gtczjrwstj.html

[R48] awk 取指定列
来源：http://hz.ydjk.org.cn/gtigdfrdbo.html

awk '{print $1, $3}' a.txt
来源：http://hz.fzhhl.top/gtbyonsiyf.html

[R49] awk 带条件
来源：http://hz.tanke756.top/gtdloetamf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jinghuilouyu.cn/gtodoqvyhr.html

[R50] awk 求和
来源：http://hz.svipenyu.cn/gtrmmdwsri.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.tanke756.top/gtrmgsdzsq.html

[R51] 排序去重取前几
来源：http://hz.wangdashe.top/gtckvlboll.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.tanke756.top/gtybyfblqs.html

[R52] 统计行数
来源：http://hz.tianlin.xyz/gtqdctmcuc.html

wc -l a.txt
来源：http://hz.hnxiangtu.top/gtwgniouue.html

[R53] 查看文件头与实时尾
来源：http://hz.gzhubu.top/gtcypyybxy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yuanzhike.top/gtqnwuwwkf.html

[R54] 比较两个文件
来源：http://hz.ydzc1.top/gtjltucuxf.html

diff a.txt b.txt
来源：http://hz.zhijiandao.cn/gtrtuhlcpf.html

[R55] 压缩与解压
来源：http://hz.cashguo.top/gtjneqnynu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhoulong.xyz/gtenzoombm.html

[R56] 远程拷贝
来源：http://hz.sweek.top/gtvsvjeiks.html

scp file user@host:/path/
来源：http://hz.gzhubu.top/gtreivwnpl.html

[R57] 远程执行命令
来源：http://hz.zhoulong.xyz/gtmftzvfaz.html

ssh user@host 'uptime'
来源：http://hz.xingfuxueyuan.xyz/gtbdlsbtju.html

[R58] 下载文件
来源：http://hz.shanyushiyangtech.top/gtmqnurhfo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.52xcode.cn/gtavydhdch.html

[R59] 发 POST JSON
来源：http://hz.feifeiyinyue.top/gtiaoxkrbi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhixingplan.top/gtuozpjogy.html

[R60] 只看 HTTP 状态码
来源：http://hz.cdnleiting.top/gtumyhdydu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.feifeiyinyue.top/gtlljeesqv.html

[R61] 磁盘占用
来源：http://hz.guowangkeji.top/gtxcfuyipx.html

df -h;  du -sh *
来源：http://hz.xinyue.icu/gtcikosqna.html

[R62] 找最占空间的文件
来源：http://hz.mhx1999.top/gtjrrvmfyv.html

du -ah . | sort -rh | head -10
来源：http://hz.yonumen.top/gtxnwjbxel.html

[R63] 内存与进程
来源：http://hz.xziqi.cn/gtnsbcmrrz.html

free -h;  ps aux | grep nginx
来源：http://hz.zhijiandao.cn/gtdixxrkrc.html

[R64] 结束进程
来源：http://hz.jinqigfzy.top/gtnagpaizn.html

kill -9 $(pgrep -f app.py)
来源：http://hz.tian-w.cn/gtetppdgkd.html

[R65] 查看端口占用
来源：http://hz.andypj.xyz/gtgqjwdpny.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yanxiufei.cn/gtubqmjggy.html

[R66] 定时任务
来源：http://hz.0kj1m.cn/gtxhqlyjln.html

crontab -e;  crontab -l
来源：http://hz.ppjwa.cn/gtazgnjubj.html

[R67] 生成随机十六进制串
来源：http://hz.pengpengdd.cyou/gtyvgsvigd.html

openssl rand -hex 16
来源：http://hz.xziqi.cn/gtszxqtymu.html

[R68] 计算文件校验值
来源：http://hz.redwolf501.top/gtznnqwrnn.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ppjwa.cn/gtkpililof.html

[R69] 生成随机密码
来源：http://hz.yueranfly.top/gtblnkrxih.html

head -c 16 /dev/urandom | base64
来源：http://hz.aibaodan.cn/gtbvgvpwtg.html

[R70] 时间戳与互转
来源：http://hz.zhijiandao.cn/gtirziywxy.html

date +%s;  date -d @1700000000
来源：http://hz.birdmap.top/gttwxyyvts.html

[R71] 日期格式化
来源：http://hz.hongshengwenyu.top/gtittiwhou.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.gzhubu.top/gtamitzutw.html

[R72] 等待端口就绪
来源：http://hz.jianghu66.top/gtxrmrsxaf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jinqigfzy.top/gtbbayejlg.html

[R73] 分割大日志
来源：http://hz.yj20258888.top/gtalhpjsuz.html

split -l 1000 big.log part_
来源：http://hz.shanyushiyangkeji.top/gtsrycszjt.html

[R74] 批量重命名
来源：http://hz.aizwys.cn/gtltrkviub.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ydzc1.top/gtoapyaghb.html

[R75] 导出环境变量
来源：http://hz.jinyuanbaomall.cn/gtyonumbjw.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shanyushiyangtech.top/gtzkraklpb.html

[R76] 使用临时文件
来源：http://hz.gaohongyu789.top/gtxviuytbq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.nanxuanxn.top/gtntozqdgw.html

[R77] 读取用户输入
来源：http://hz.shuidangran.top/gtcfgtxkza.html

read -rp "请输入: " ans
来源：http://hz.hfpthk.cn/gtaiblefbj.html

[R78] 交互式菜单
来源：http://hz.9152youxi.cn/gtqraqwwhi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hammf.cn/gttgybibob.html

[R79] 解析命令行选项
来源：http://hz.yuxming.cn/gtjtllsiks.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.feifeiyinyue.top/gtrxftitcs.html

[R80] 查看脚本执行耗时
来源：http://hz.jqgufenzy.top/gtzcnztqoi.html

time ./run.sh
来源：http://hz.gogol.net.cn/gtuiybwdwj.html

================================================================================
来源：http://hz.yuxming.cn/gtwfeykoxm.html

S. C / C++ 专题
来源：http://hz.zycfv.cn/gtnxlgibxl.html

================================================================================
来源：http://hz.aizwys.cn/gtkgcgeqaf.html

[S01] C：Hello World
来源：http://hz.haohaochexian.top/gtrrwqmgri.html

#include <stdio.h>
来源：http://hz.chenjidiqi.icu/gtifcpktue.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jiagoushi.top/gtdsabldbf.html

[S02] C：变量与格式化输出
来源：http://hz.tian-w.cn/gteohdhidn.html

int a = 10; printf("%d\n", a);
来源：http://hz.aizwys.cn/gtlpvpwttz.html

[S03] C：读入整数
来源：http://hz.yangfankeji.com/gtpqqesuda.html


<!-- 参考信息 -->