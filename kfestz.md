代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.chenzaomai.com/gtalyrlifg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.9152youxi.cn/gttnqqobpc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.9152youxi.cn/gtssywlfla.html

[Q41] 多表连接
来源：http://hz.hongshengwenyu.top/gtjiodimjb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xziqi.cn/gtkeavaibm.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xuanzx.com/gtqkfsusgx.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yuanzhike.top/gtpqcjwcew.html

[Q42] 连接条件附加过滤
来源：http://hz.cdnleiting.top/gthugoebyg.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ywan-chungtsiang.top/gtseeotlnv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.52xcode.cn/gtxacfexip.html

[Q43] 标量子查询
来源：http://hz.chenzaomai.com/gthskauzte.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.gogol.net.cn/gtgsfpkkch.html

[Q44] IN 子查询
来源：http://hz.ybcxt.top/gtmikolxis.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.feifeiyinyue.top/gtyhkjvrqb.html

[Q45] EXISTS 判断存在
来源：http://hz.kuanghao11.cn/gtiilbtazg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shanyushiyangtech.top/gtbqowwwvq.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.9152youxi.cn/gtxmavytab.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ybcxt.top/gtpgtwoxuy.html

[Q47] 与平均值比较
来源：http://hz.yongpay.top/gthkoxhclw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhaomingkeji.xyz/gteostwkrp.html

[Q48] CTE 公用表表达式
来源：http://hz.pengpengdd.cyou/gtmmepuvdi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jyoumei.cn/gtwauwkldg.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.iojbl.cn/gtumeyxhxp.html

[Q49] 更新单行
来源：http://hz.snrcjt.cn/gtoukrkvdu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.sweek.top/gtimlgqaam.html

[Q50] 批量更新
来源：http://hz.jyoumei.cn/gtsjbsthas.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.shzxlz.cn/gtlvyrbsaf.html

[Q51] 用子查询更新
来源：http://hz.meibo888.top/gtaleuvpnx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ywan-chungtsiang.top/gtyldncopy.html

[Q52] 删除指定行
来源：http://hz.cashguo.top/gtortfdeai.html

DELETE FROM users WHERE id = 10;
来源：http://hz.cashguo.top/gtltqbcawu.html

[Q53] 按条件删除
来源：http://hz.tian-w.cn/gtfqdrpzhi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.guannengcc.top/gtcxmriqkg.html

[Q54] 清空表
来源：http://hz.wangdashe.top/gtobowzmwf.html

TRUNCATE TABLE logs;
来源：http://hz.zhengqikj.top/gtukgsdgpy.html

[Q55] 排名（并列占位）
来源：http://hz.jianghu66.top/gtcpniiqqd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.9152youxi.cn/gtpvmaloon.html

[Q56] 密集排名（并列不占位）
来源：http://hz.guannengcc.top/gtflgiwmtj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.tianlin.xyz/gtbtsnkirh.html

[Q57] 行号
来源：http://hz.yonumen.top/gtzhwvcrwt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cucudq.cn/gtqawogyfs.html

[Q58] 累计求和
来源：http://hz.xuetiantiany.cn/gtiflshcrc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cqqwz.cn/gtqswkmhpb.html

[Q59] 分组内累计
来源：http://hz.pengpengdd.cyou/gtlsdwwvbs.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.tanke756.top/gtrucookzj.html

[Q60] 取上一行 / 下一行
来源：http://hz.aizwys.cn/gttqreficv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.iojbl.cn/gtxukoeeye.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yangfankeji.com/gtselagxzp.html

[Q61] 移动平均
来源：http://hz.shanyushiyangkeji.top/gthyyutqpp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xuetiantiany.cn/gtarnnktez.html

[Q62] 分组占比
来源：http://hz.shanyushiyangkeji.top/gtnrfrhdpp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.xuanzx.com/gtjomcwvbb.html

[Q63] 开启事务
来源：http://hz.fengsongda.top/gtczrsugcz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shzxlz.cn/gtbajxgwfa.html

[Q64] 提交事务
来源：http://hz.pycfn.com/gtazykkzjv.html

COMMIT;
来源：http://hz.haohaochexian.top/gtqloxraio.html

[Q65] 回滚事务
来源：http://hz.cashguo.top/gtqpsgfhud.html

ROLLBACK;
来源：http://hz.0kj1m.cn/gttzdtwuld.html

[Q66] 行锁查询
来源：http://hz.svipenyu.cn/gtnaekvjep.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.meibo888.top/gtbyfqqgzi.html

[Q67] 设置隔离级别
来源：http://hz.nwbrower.top/gtbrpoimlm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.xinyue.icu/gtlfknpkkj.html

[Q68] 保存点
来源：http://hz.yj202588.top/gtpoaadksz.html

SAVEPOINT sp1;
来源：http://hz.zhijiandao.cn/gtljniembb.html

ROLLBACK TO sp1;
来源：http://hz.shanyushiyangkeji.top/gtfymswxra.html

[Q69] 查看执行计划
来源：http://hz.gzhubu.top/gtuhsgcggi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.cheryme.top/gtjpeojsox.html

[Q70] 更新统计信息
来源：http://hz.yj20258888.top/gtnnlipwku.html

ANALYZE TABLE users;
来源：http://hz.tian-w.cn/gtnbvwocrc.html

[Q71] 查看建表语句
来源：http://hz.shanyushiyangtech.top/gtswyxjjjv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.sufxvd.cn/gtqgulboqt.html

[Q72] 查看索引
来源：http://hz.dianchejie.cn/gtpkdfobsa.html

SHOW INDEX FROM users;
来源：http://hz.havefunace.top/gtvhvomdow.html

[Q73] 查看表状态
来源：http://hz.kuanghao11.cn/gtpnevbwde.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zdqjudy.top/gtakktayhe.html

[Q74] 强制使用索引
来源：http://hz.jqgfzy.top/gtjerxrfde.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.nanxuanxn.top/gtrkhjcfvn.html

[Q75] 日期格式化
来源：http://hz.iojbl.cn/gtnyunplhh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.52xcode.cn/gtktaunnqk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.tianlin.xyz/gtmopswklp.html

[Q76] 按天统计
来源：http://hz.jinqigufen.top/gtsxaaalyt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sufxvd.cn/gttrrdcrqt.html

[Q77] 时间加减
来源：http://hz.gogol.net.cn/gtsylwoybf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.dianchejie.cn/gtjyxaoegs.html

[Q78] 当前时间
来源：http://hz.svipenyu.cn/gtlzkpcqip.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jiagoushi.top/gtqmdrvirs.html

[Q79] 字符串拼接
来源：http://hz.hywenlv.cn/gtacumrzkg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jianghu66.top/gtaejmfnzx.html

[Q80] 字符串截取
来源：http://hz.birdmap.top/gthbpmuxbg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhaomingkeji.xyz/gtzeessycf.html

[Q81] 字符串替换
来源：http://hz.tian-w.cn/gtetrfcvbi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhixingplan.top/gtcsbhmbxm.html

[Q82] 字符长度与字节长度
来源：http://hz.pengpengdd.cyou/gtujvozriz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yj20258888.top/gtbgsuciiy.html

[Q83] 大小写转换
来源：http://hz.zhongyouzk.top/gtnimoqxqk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.birdmap.top/gtcjhwwtnx.html

[Q84] 去除首尾空格
来源：http://hz.sysykeji.top/gtwtpvmfmw.html

SELECT TRIM(name) FROM users;
来源：http://hz.svipenyu.cn/gthxyqkzcj.html

[Q85] 数值取整
来源：http://hz.pycfn.com/gtuvoygryg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.gogol.net.cn/gtpailshpl.html

[Q86] 读取 JSON 字段
来源：http://hz.daria6918.cn/gtkksjlhss.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hysaishi.cn/gtqcekpnjt.html

[Q87] JSON 字段做条件
来源：http://hz.yuanzhike.top/gtwlixjhri.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zycfv.cn/gtpfcatcai.html

[Q88] 行转列（条件聚合）
来源：http://hz.yj20258888.top/gtgmtbuwhn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.daxiang520.top/gtckzhhvbp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yonumen.top/gtfdjmuezo.html

[Q89] 判断表是否存在
来源：http://hz.jyoumei.cn/gtzdrlmpub.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zycfv.cn/gtagnevdtb.html

[Q90] 生成序号列
来源：http://hz.hammf.cn/gtrgnayxon.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xuetiantiany.cn/gtiytzdvhi.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtocniqxpo.html

R. Bash 专题
来源：http://hz.gaohongyu789.top/gttadflaak.html

================================================================================
来源：http://hz.bjfxy.top/gtjioyjixy.html

[R01] shebang 与严格模式
来源：http://hz.dashuyun.cn/gtxvqfzhjc.html

#!/usr/bin/env bash
来源：http://hz.jinyuanbaomall.cn/gtchbuirfh.html

set -euo pipefail
来源：http://hz.gzhubu.top/gtcigyffhq.html

[R02] 变量赋值与使用
来源：http://hz.zhoulong.xyz/gtmrskrpav.html

name="Tom"; echo "$name"
来源：http://hz.hnqzz.top/gtvkshvhwq.html

[R03] 只读变量
来源：http://hz.daria6918.cn/gtaesuaafb.html

readonly PI=3.14
来源：http://hz.zhongyouzk.top/gtnhgzbamz.html

[R04] 位置参数
来源：http://hz.pengpengdd.cyou/gtibkkglbe.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jinghuilouyu.cn/gtipjcbxas.html

[R05] 参数默认值
来源：http://hz.bjfxy.top/gtnrefgsfl.html

name="${1:-default}"
来源：http://hz.wangshuangyany.cn/gtalzpvhrv.html

[R06] 判断命令是否存在
来源：http://hz.fzhhl.top/gtjlesfbgs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.svipenyu.cn/gtwtkjkhjz.html

[R07] if 判断文件
来源：http://hz.vqdsnc.cn/gtysrxdswj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.dashuyun.cn/gtsqvovrad.html

[R08] 数值比较
来源：http://hz.cucudq.cn/gtwrbraxmw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yongpay.top/gtfofaxezw.html

[R09] 字符串比较
来源：http://hz.fzhhl.top/gtfveuambx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xuanzx.com/gtalthiwft.html

[R10] 正则匹配
来源：http://hz.dashuyun.cn/gtzyitrrde.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.pengpengdd.cyou/gtrmtmqvjq.html

[R11] case 多分支
来源：http://hz.jinghuilouyu.cn/gticrtaxnd.html

case "$1" in
来源：http://hz.9152youxi.cn/gtynwzltqh.html

start) echo "启动" ;;
来源：http://hz.tanke756.top/gtvheabakj.html

stop)  echo "停止" ;;
来源：http://hz.c1oappe.top/gtpzbhoikf.html

*)     echo "未知命令" ;;
来源：http://hz.hongshengwenyu.top/gtddzgmxnk.html

esac
来源：http://hz.jqgfzy.top/gtrxgtjlpd.html

[R12] for 遍历文件
来源：http://hz.sweek.top/gtrulruwst.html

for f in *.txt; do echo "$f"; done
来源：http://hz.wangdashe.top/gtglajxykq.html

[R13] for 计数循环
来源：http://hz.gotoacloud.top/gtzkbohrme.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yj20258.top/gtlvamhpof.html

[R14] C 风格 for
来源：http://hz.gzhubu.top/gtrlegmnio.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.svipenyu.cn/gthtgupcjz.html

[R15] while 逐行读文件
来源：http://hz.mhx1999.top/gtuecgsfmc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zdqjudy.top/gthnvovqsm.html

[R16] until 等待条件
来源：http://hz.dashuyun.cn/gtekgdbbde.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.fengsongda.top/gthhzsfsei.html

[R17] 数组定义与取值
来源：http://hz.ywan-chungtsiang.top/gtvltvulmc.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hnxiangtu.top/gthoiotqgu.html

[R18] 遍历数组
来源：http://hz.xylfe.cn/gtzrbasklp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yonumen.top/gtnhfrkkxn.html

[R19] 数组长度
来源：http://hz.aibaodan.cn/gtuwmjgsih.html

echo "${#arr[@]}"
来源：http://hz.yueranfly.top/gtuhafhnhm.html

[R20] 关联数组（字典）
来源：http://hz.yueranfly.top/gtznvwmqgm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.sweek.top/gtjzpswvzm.html

[R21] 字符串长度
来源：http://hz.xinyue.icu/gthrblyqzu.html

echo "${#s}"
来源：http://hz.jianghu66.top/gtqpumczob.html

[R22] 截取子串
来源：http://hz.wangdashe.top/gtwbtngynu.html

echo "${s:0:5}"
来源：http://hz.snrcjt.cn/gtcapyjirr.html

[R23] 字符串替换
来源：http://hz.svipenyu.cn/gtsfngfrjx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.dashuyun.cn/gtojihnbrz.html

[R24] 大小写转换
来源：http://hz.wangdashe.top/gtwcqzntoj.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.fengsongda.top/gthxtffwyk.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhaomingkeji.xyz/gtxnbbnfyc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yanxiufei.cn/gtaodrhshh.html

[R26] 命令替换
来源：http://hz.sufxvd.cn/gtmlskqzpi.html

now=$(date +%F); echo "$now"
来源：http://hz.smart0.xyz/gtutcqpbgk.html

[R27] 算术展开
来源：http://hz.nanxinkj.top/gthhfcpeio.html

echo $((1 + 2 * 3))
来源：http://hz.ybcxt.top/gtujpmbhxr.html

[R28] 浮点运算
来源：http://hz.ydjk.org.cn/gtrlhshqqf.html

echo "scale=2; 10/3" | bc
来源：http://hz.sweek.top/gtgqdcefsx.html

[R29] 定义函数
来源：http://hz.shzxlz.cn/gtmrjvxqjr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yonumen.top/gtasojqbqw.html

[R30] 函数返回状态码
来源：http://hz.pycfn.com/gtjiieemax.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.chenjidiqi.icu/gtkgqzzqkm.html

[R31] 局部变量
来源：http://hz.svipenyu.cn/gtgcsegxhc.html

f() { local x=1; echo "$x"; }
来源：http://hz.xingfuxueyuan.xyz/gtwenzfkbq.html

[R32] 参数个数校验
来源：http://hz.52xcode.cn/gtzhzcffwl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.0kj1m.cn/gtcoqiiyuq.html

[R33] 捕获错误并提示行号
来源：http://hz.c1oappe.top/gtydrffdgo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xylfe.cn/gtacilmata.html

[R34] 退出时清理
来源：http://hz.ywan-chungtsiang.top/gtirubvrql.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinqigfzy.top/gtjysbreyl.html

[R35] 后台执行并等待
来源：http://hz.ywan-chungtsiang.top/gttxpboewu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xuanzx.com/gtspruopai.html

[R36] 并发执行多个任务
来源：http://hz.yj202588.top/gtgqqxgruo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.52xcode.cn/gtipvdtzrx.html

[R37] 把输出赋给变量
来源：http://hz.nanxuanxn.top/gtnjcpchyx.html

files=$(ls -1)
来源：http://hz.zhengqikj.top/gtonssvzur.html

[R38] 管道串联
来源：http://hz.jianghu66.top/gtmjzggrrf.html

cat a.txt | grep -i error | wc -l
来源：http://hz.feifeiyinyue.top/gtsbpiycxi.html

[R39] 重定向标准输出与错误
来源：http://hz.cqqwz.cn/gtfiomcphb.html

cmd > out.log 2>&1
来源：http://hz.fzhhl.top/gthvazrtou.html

[R40] 追加写日志
来源：http://hz.sufxvd.cn/gtpwkwhgjg.html

echo "log" >> out.log
来源：http://hz.iojbl.cn/gtbctjjzbf.html

[R41] 丢弃输出
来源：http://hz.yj20258.top/gtqdiabmup.html

cmd >/dev/null 2>&1
来源：http://hz.nanxinkj.top/gtcvhkeogv.html

[R42] 输入重定向
来源：http://hz.jinqigfzy.top/gthahcmhku.html

wc -l < a.txt
来源：http://hz.fengsongda.top/gtvrfwsexa.html

[R43] 按名字查找文件
来源：http://hz.shanyushiyangtech.top/gtaakkiwdn.html

find . -name "*.log" -type f
来源：http://hz.jqgufenzy.top/gtskxwnuay.html

[R44] 按修改时间查找
来源：http://hz.wangdashe.top/gteyifumep.html

find . -mtime -7 -type f
来源：http://hz.vqdsnc.cn/gtthwjrnuq.html

[R45] 批量删除
来源：http://hz.fzhhl.top/gtwyzihwkj.html

find . -name "*.tmp" -delete
来源：http://hz.c1oappe.top/gtxemfpzoq.html

[R46] 递归替换文件内容
来源：http://hz.hongshengwenyu.top/gtxxtvikrk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yvedp.cn/gtsztcphju.html

[R47] sed 单行替换
来源：http://hz.c1oappe.top/gtsluiaaqc.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hongshengwenyu.top/gtrdudqwhd.html

[R48] awk 取指定列
来源：http://hz.cdnleiting.top/gtnqrlmunn.html

awk '{print $1, $3}' a.txt
来源：http://hz.fzhhl.top/gtrvijrlpa.html

[R49] awk 带条件
来源：http://hz.tian-w.cn/gtpmlpowab.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhixingplan.top/gtcnvsuodx.html

[R50] awk 求和
来源：http://hz.cashguo.top/gtckbtaphz.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xingfuxueyuan.xyz/gtyfixpbta.html

[R51] 排序去重取前几
来源：http://hz.shanyushiyangkeji.top/gtlerlvmda.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shzxlz.cn/gtpzrdqjlt.html

[R52] 统计行数
来源：http://hz.ywan-chungtsiang.top/gtirefeghj.html

wc -l a.txt
来源：http://hz.dianchejie.cn/gtpwgifguq.html

[R53] 查看文件头与实时尾
来源：http://hz.guowangkeji.top/gtomchbdko.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yuxming.cn/gtkjkvaygd.html

[R54] 比较两个文件
来源：http://hz.zycfv.cn/gtpjcruews.html

diff a.txt b.txt
来源：http://hz.ppjwa.cn/gtaqmthvgn.html

[R55] 压缩与解压
来源：http://hz.xingfuxueyuan.xyz/gtqvmzjduu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.daria6918.cn/gthgagzsoj.html

[R56] 远程拷贝
来源：http://hz.nanxuanxn.top/gtqhqwjakt.html

scp file user@host:/path/
来源：http://hz.dashuyun.cn/gtsdnajjtp.html

[R57] 远程执行命令
来源：http://hz.yj20258.top/gtqahqiquc.html

ssh user@host 'uptime'
来源：http://hz.daria6918.cn/gtuqelahob.html

[R58] 下载文件
来源：http://hz.zhijiandao.cn/gtrojlxcxi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.chenzaomai.com/gtbkvtsaja.html

[R59] 发 POST JSON
来源：http://hz.zycfv.cn/gtgwicipav.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shangyingyoupin.top/gtyhcsbtgm.html

[R60] 只看 HTTP 状态码
来源：http://hz.jinghuilouyu.cn/gtfozcfevm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yuxming.cn/gtotjapvot.html

[R61] 磁盘占用
来源：http://hz.zhixingplan.top/gtpumxbmex.html

df -h;  du -sh *
来源：http://hz.havefunace.top/gtuwyrnvno.html

[R62] 找最占空间的文件
来源：http://hz.316326.xyz/gtnxgtbtsd.html

du -ah . | sort -rh | head -10
来源：http://hz.pengpengdd.cyou/gtrmbuijzy.html

[R63] 内存与进程
来源：http://hz.yj202588.top/gtqogzwjpb.html

free -h;  ps aux | grep nginx
来源：http://hz.xziqi.cn/gtnyuxzmvj.html

[R64] 结束进程
来源：http://hz.jinyuanbaomall.cn/gtzdqzecbp.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hfpthk.cn/gtypblsutp.html

[R65] 查看端口占用
来源：http://hz.hysaishi.cn/gtvrajdogh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.nwbrower.top/gtvfuksrxp.html

[R66] 定时任务
来源：http://hz.jiagoushi.top/gtohetbffr.html

crontab -e;  crontab -l
来源：http://hz.birdmap.top/gtwugemiee.html

[R67] 生成随机十六进制串
来源：http://hz.chenzaomai.com/gtjwjakuoo.html

openssl rand -hex 16
来源：http://hz.daxiang520.top/gtdigbbdzf.html

[R68] 计算文件校验值
来源：http://hz.meibo888.top/gtnrkhsqgl.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xylfe.cn/gthwhyeryd.html

[R69] 生成随机密码
来源：http://hz.nanxuanxn.top/gtayxixyom.html

head -c 16 /dev/urandom | base64
来源：http://hz.hywenlv.cn/gtaqgneprf.html

[R70] 时间戳与互转
来源：http://hz.zhiwuduotai.top/gtuljufzsl.html

date +%s;  date -d @1700000000
来源：http://hz.vqdsnc.cn/gtdguywiyu.html

[R71] 日期格式化
来源：http://hz.hysaishi.cn/gthmjdrtcc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shanyushiyangtech.top/gtkpasbxqe.html

[R72] 等待端口就绪
来源：http://hz.hnxiangtu.top/gtorevtanu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.cucudq.cn/gtjoyoqzhb.html

[R73] 分割大日志
来源：http://hz.yj202588.top/gtumcapnta.html

split -l 1000 big.log part_
来源：http://hz.jiagoushi.top/gtwffgszlc.html

[R74] 批量重命名
来源：http://hz.hysaishi.cn/gtuokyojpc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jqgufenzy.top/gttspxemge.html

[R75] 导出环境变量
来源：http://hz.snrcjt.cn/gtwhjvfekm.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shzxlz.cn/gtvdcmfwmt.html

[R76] 使用临时文件
来源：http://hz.zdqjudy.top/gtvhyixyor.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yonumen.top/gtwxqynqrl.html

[R77] 读取用户输入
来源：http://hz.hnqzz.top/gtlzvtrdbk.html

read -rp "请输入: " ans
来源：http://hz.zhongyouzk.top/gthjazayur.html

[R78] 交互式菜单
来源：http://hz.daxiang520.top/gtszvsawen.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.gotoacloud.top/gtqfpulwyi.html

[R79] 解析命令行选项
来源：http://hz.sufxvd.cn/gtguigjuse.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.cucudq.cn/gtokasaslj.html

[R80] 查看脚本执行耗时
来源：http://hz.tanke756.top/gtwzsmtixd.html

time ./run.sh
来源：http://hz.cheryme.top/gtmakjqyvn.html

================================================================================
来源：http://hz.havefunace.top/gtgdqpevvm.html

S. C / C++ 专题
来源：http://hz.chenlongwang.top/gtcfkovczz.html

================================================================================
来源：http://hz.hysaishi.cn/gtrbdjzvhv.html

[S01] C：Hello World
来源：http://hz.daxiang520.top/gtlsjzjkwk.html

#include <stdio.h>
来源：http://hz.tianlin.xyz/gtflatiada.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xuanzx.com/gtpogkqoqx.html

[S02] C：变量与格式化输出
来源：http://hz.xylfe.cn/gtkdjueakt.html

int a = 10; printf("%d\n", a);
来源：http://hz.ydzc1.top/gtbruccmtc.html

[S03] C：读入整数
来源：http://hz.xylfe.cn/gteeqyztlz.html

int x; scanf("%d", &x);
来源：http://hz.andypj.xyz/gtpknnsiyr.html

[S04] C：字符串复制
来源：http://hz.hnqzz.top/gtbwjhrsyg.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.vqdsnc.cn/gthahebnhx.html

[S05] C：字符串长度
来源：http://hz.daria6918.cn/gtcmsydbdv.html

strlen(s)
来源：http://hz.ehwqpu.com/gtnsuhpsnx.html

[S06] C：字符串比较
来源：http://hz.sweek.top/gtjyioetgf.html

strcmp(a, b) == 0
来源：http://hz.xylfe.cn/gtzyzasnwa.html

[S07] C：数组遍历求和
来源：http://hz.vqdsnc.cn/gtzefgpjst.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jqgufenzy.top/gtbjzjapqn.html

[S08] C：动态内存分配与释放
来源：http://hz.nanxuanxn.top/gtmikujqvx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.gaohongyu789.top/gtnvzkbsgx.html

[S09] C：结构体定义与初始化
来源：http://hz.jinqigfzy.top/gtgppnhlor.html


<!-- 参考信息 -->