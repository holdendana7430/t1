代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yangfankeji.com/gtdzjdlzdb.html

[Q50] 批量更新
来源：http://hz.sxryk.cn/gtwiosspbi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yueranfly.top/gtjdtimofi.html

[Q51] 用子查询更新
来源：http://hz.havefunace.top/gtjkvsutvw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jlsjyb.cn/gtniwybmdl.html

[Q52] 删除指定行
来源：http://hz.c1oappe.top/gtgvucvthy.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhongyouzk.top/gtovylhedx.html

[Q53] 按条件删除
来源：http://hz.aizwys.cn/gtugicnmnm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.guowangkeji.top/gtbglfoysu.html

[Q54] 清空表
来源：http://hz.jianghu66.top/gtjcwaiuzi.html

TRUNCATE TABLE logs;
来源：http://hz.xinyue.icu/gtkgtokuml.html

[Q55] 排名（并列占位）
来源：http://hz.havefunace.top/gtgciisuoh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhijiandao.cn/gtgyjwzrvf.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ywan-chungtsiang.top/gtpyuehmno.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jianghu66.top/gtiigvshni.html

[Q57] 行号
来源：http://hz.chenjidiqi.icu/gteurgokuq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ydjk.org.cn/gtzhetzxlj.html

[Q58] 累计求和
来源：http://hz.yuanzhike.top/gtxdayxfxn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yanxiufei.cn/gtspyosbzv.html

[Q59] 分组内累计
来源：http://hz.ywan-chungtsiang.top/gtxzhfqqkk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yueranfly.top/gtuegmwhxr.html

[Q60] 取上一行 / 下一行
来源：http://hz.sxryk.cn/gtaintddwm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.xylfe.cn/gtaocsfsnr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.chenjidiqi.icu/gtdorriycf.html

[Q61] 移动平均
来源：http://hz.xinyue.icu/gtimqswulc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.cheryme.top/gtshbafxsz.html

[Q62] 分组占比
来源：http://hz.shzxlz.cn/gtcuhwgvjs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.0kj1m.cn/gtkkkwhugv.html

[Q63] 开启事务
来源：http://hz.zdqjudy.top/gtqocysavh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.cqqwz.cn/gtrhbellfz.html

[Q64] 提交事务
来源：http://hz.guowangkeji.top/gtjggxsvis.html

COMMIT;
来源：http://hz.zhoulong.xyz/gtgnigelgq.html

[Q65] 回滚事务
来源：http://hz.gogol.net.cn/gtlwbmfwvc.html

ROLLBACK;
来源：http://hz.ppjwa.cn/gtlhogrxcd.html

[Q66] 行锁查询
来源：http://hz.nanxuanxn.top/gtktqejonp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hnqzz.top/gthmwzophk.html

[Q67] 设置隔离级别
来源：http://hz.cdnleiting.top/gtqeesjzym.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ydzc1.top/gtkmajoxjd.html

[Q68] 保存点
来源：http://hz.guannengcc.top/gtlgsrzley.html

SAVEPOINT sp1;
来源：http://hz.sweek.top/gtsztuaxse.html

ROLLBACK TO sp1;
来源：http://hz.yongpay.top/gtbqqlyyyc.html

[Q69] 查看执行计划
来源：http://hz.mhx1999.top/gtvckymkuh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.nwbrower.top/gtslatvjgk.html

[Q70] 更新统计信息
来源：http://hz.jqgfzy.top/gtwmrkqzfl.html

ANALYZE TABLE users;
来源：http://hz.sysykeji.top/gtagytmwba.html

[Q71] 查看建表语句
来源：http://hz.aibaodan.cn/gtwcsrxdoh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.daria6918.cn/gtudcjpkzo.html

[Q72] 查看索引
来源：http://hz.jqgufenzy.top/gtfprkqtry.html

SHOW INDEX FROM users;
来源：http://hz.andypj.xyz/gtjiiwvdpy.html

[Q73] 查看表状态
来源：http://hz.meibo888.top/gtsglmpzty.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.iojbl.cn/gtkzxqcnyx.html

[Q74] 强制使用索引
来源：http://hz.xziqi.cn/gtsuzvoyuf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.redwolf501.top/gtxopepbyr.html

[Q75] 日期格式化
来源：http://hz.zhijiandao.cn/gtuodbhbzx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.nwbrower.top/gtcurjrecp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ywan-chungtsiang.top/gtxvqluvvm.html

[Q76] 按天统计
来源：http://hz.smart0.xyz/gthogifhtq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.hnxiangtu.top/gthvlxadns.html

[Q77] 时间加减
来源：http://hz.ydzc1.top/gtvbdtjhbg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nanxinkj.top/gtqtrtegxa.html

[Q78] 当前时间
来源：http://hz.jinyuanbaomall.cn/gtzflxyjgs.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.gaohongyu789.top/gtjwveylhg.html

[Q79] 字符串拼接
来源：http://hz.tian-w.cn/gtcwptcvqu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jiagoushi.top/gttggfsqnb.html

[Q80] 字符串截取
来源：http://hz.nanxinkj.top/gtbpwdkbzu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yj202588.top/gthpdapfth.html

[Q81] 字符串替换
来源：http://hz.hysaishi.cn/gtqikfcevs.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.guannengcc.top/gtyqaeeaxh.html

[Q82] 字符长度与字节长度
来源：http://hz.aibaodan.cn/gtrivxtsju.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.wangdashe.top/gtjezssegd.html

[Q83] 大小写转换
来源：http://hz.hywenlv.cn/gtjwhtjjmp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.shangyingyoupin.top/gtvnwzungm.html

[Q84] 去除首尾空格
来源：http://hz.meibo888.top/gtaapjyqap.html

SELECT TRIM(name) FROM users;
来源：http://hz.daxiang520.top/gtmzgscbfd.html

[Q85] 数值取整
来源：http://hz.yueranfly.top/gtdgfbxmfd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.shangyingyoupin.top/gtdttqtckd.html

[Q86] 读取 JSON 字段
来源：http://hz.gogol.net.cn/gtuanmskiu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.andypj.xyz/gtuapiutpr.html

[Q87] JSON 字段做条件
来源：http://hz.zycfv.cn/gtfndiqknm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yongpay.top/gtzmofxhvu.html

[Q88] 行转列（条件聚合）
来源：http://hz.aibaodan.cn/gtcsgknxde.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.xziqi.cn/gtqqsjnosh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.aibaodan.cn/gtxepqrxem.html

[Q89] 判断表是否存在
来源：http://hz.hammf.cn/gtfxfenood.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yuxming.cn/gtjlgftuvz.html

[Q90] 生成序号列
来源：http://hz.jianghu66.top/gtnlskwzim.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zycfv.cn/gtubelpamc.html

================================================================================
来源：http://hz.iojbl.cn/gtvioylxjc.html

R. Bash 专题
来源：http://hz.xingfuxueyuan.xyz/gtbxvbzqbr.html

================================================================================
来源：http://hz.jiagoushi.top/gtpkcbvuib.html

[R01] shebang 与严格模式
来源：http://hz.xinyue.icu/gtlqjwrcvz.html

#!/usr/bin/env bash
来源：http://hz.chenzaomai.com/gtljmqobcg.html

set -euo pipefail
来源：http://hz.quarkkingdee.top/gtzeqfburu.html

[R02] 变量赋值与使用
来源：http://hz.c1oappe.top/gtsrzauffs.html

name="Tom"; echo "$name"
来源：http://hz.daxiang520.top/gtputuoadw.html

[R03] 只读变量
来源：http://hz.chenlongwang.top/gtrlljqybg.html

readonly PI=3.14
来源：http://hz.xziqi.cn/gtccuhbgky.html

[R04] 位置参数
来源：http://hz.xingfuxueyuan.xyz/gtyifeixgs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xziqi.cn/gtvtxqshep.html

[R05] 参数默认值
来源：http://hz.jinqigufen.top/gtosufqkwh.html

name="${1:-default}"
来源：http://hz.jyoumei.cn/gtjwkmqekf.html

[R06] 判断命令是否存在
来源：http://hz.tianlin.xyz/gtaecfdaog.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.nanxuanxn.top/gtiyufbkwe.html

[R07] if 判断文件
来源：http://hz.yvedp.cn/gtzzrnrhzb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.pengpengdd.cyou/gthtmzlmqp.html

[R08] 数值比较
来源：http://hz.guowangkeji.top/gtwdztlgif.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.quarkkingdee.top/gtghkrtwqw.html

[R09] 字符串比较
来源：http://hz.quarkkingdee.top/gtrwyncatf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yongpay.top/gtgfeuxnkn.html

[R10] 正则匹配
来源：http://hz.yj20258.top/gthdawzdek.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.52xcode.cn/gtladxocks.html

[R11] case 多分支
来源：http://hz.smart0.xyz/gtpbaukfmm.html

case "$1" in
来源：http://hz.zhoulong.xyz/gtvfhvhdeg.html

start) echo "启动" ;;
来源：http://hz.yangfankeji.com/gtoctovinh.html

stop)  echo "停止" ;;
来源：http://hz.dianchejie.cn/gtjpsokrzo.html

*)     echo "未知命令" ;;
来源：http://hz.kuanghao11.cn/gtqbxfazqg.html

esac
来源：http://hz.xingfuxueyuan.xyz/gtvxxtcvnn.html

[R12] for 遍历文件
来源：http://hz.nanxinkj.top/gtyfyedybc.html

for f in *.txt; do echo "$f"; done
来源：http://hz.pengpengdd.cyou/gtkqfmplqa.html

[R13] for 计数循环
来源：http://hz.zhengqikj.top/gtvznnkrnb.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.chenjidiqi.icu/gtjofiaqbu.html

[R14] C 风格 for
来源：http://hz.quarkkingdee.top/gtpruyiemj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.chenjidiqi.icu/gtecacbicw.html

[R15] while 逐行读文件
来源：http://hz.ybcxt.top/gtxqeewpeh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yj202588.top/gtutvxsgfj.html

[R16] until 等待条件
来源：http://hz.cqqwz.cn/gtmifvbens.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.nanxuanxn.top/gtxkshnqxo.html

[R17] 数组定义与取值
来源：http://hz.gogol.net.cn/gtkyiuqfgf.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ehwqpu.com/gtexceopum.html

[R18] 遍历数组
来源：http://hz.hysaishi.cn/gtlisglyan.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.nwbrower.top/gtcqnrarny.html

[R19] 数组长度
来源：http://hz.haohaochexian.top/gtbmftjwwq.html

echo "${#arr[@]}"
来源：http://hz.cucudq.cn/gtmsiruvyt.html

[R20] 关联数组（字典）
来源：http://hz.hnqzz.top/gtjrryqwfw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhijiandao.cn/gtsjxlsyzh.html

[R21] 字符串长度
来源：http://hz.yuxming.cn/gtznffvcns.html

echo "${#s}"
来源：http://hz.jinyuanbaomall.cn/gtzdwvpzno.html

[R22] 截取子串
来源：http://hz.jqgfzy.top/gtoajzlqsq.html

echo "${s:0:5}"
来源：http://hz.zhengqikj.top/gtetgcehtg.html

[R23] 字符串替换
来源：http://hz.yj20258888.top/gtwirhznfc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shanyushiyangtech.top/gttazexwpw.html

[R24] 大小写转换
来源：http://hz.zdqjudy.top/gtqpleywlo.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.cdnleiting.top/gtnoreutwy.html

[R25] 去后缀 / 去前缀
来源：http://hz.zdqjudy.top/gtxtlypcgs.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.chenzaomai.com/gtpfvzojcw.html

[R26] 命令替换
来源：http://hz.aibaodan.cn/gtoqynxutc.html

now=$(date +%F); echo "$now"
来源：http://hz.jlsjyb.cn/gtbikaqumy.html

[R27] 算术展开
来源：http://hz.haohaochexian.top/gtqxyezxzb.html

echo $((1 + 2 * 3))
来源：http://hz.yuanzhike.top/gtjytscuax.html

[R28] 浮点运算
来源：http://hz.nwbrower.top/gtyjcflvtv.html

echo "scale=2; 10/3" | bc
来源：http://hz.xylfe.cn/gtsvhncehg.html

[R29] 定义函数
来源：http://hz.yuanzhike.top/gtzaognvjr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.nwbrower.top/gtuqoiwptp.html

[R30] 函数返回状态码
来源：http://hz.jinqigfzy.top/gtuqffqazm.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hfpthk.cn/gthftidbgy.html

[R31] 局部变量
来源：http://hz.guowangkeji.top/gtnnxizeal.html

f() { local x=1; echo "$x"; }
来源：http://hz.hnxiangtu.top/gthiikxgks.html

[R32] 参数个数校验
来源：http://hz.sweek.top/gtllbwmvyz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.shanyushiyangkeji.top/gtqnhjnzbh.html

[R33] 捕获错误并提示行号
来源：http://hz.dashuyun.cn/gtzprrrlzf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ivvv.top/gtcdcqlhvt.html

[R34] 退出时清理
来源：http://hz.9152youxi.cn/gtdzxqcmbk.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenzaomai.com/gtjoodbyec.html

[R35] 后台执行并等待
来源：http://hz.hfpthk.cn/gtdnsrpgwg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.tian-w.cn/gtijqpzcbt.html

[R36] 并发执行多个任务
来源：http://hz.kuanghao11.cn/gtnpmmydiu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shangyingyoupin.top/gtmzyvixwl.html

[R37] 把输出赋给变量
来源：http://hz.zycfv.cn/gtgzeithxt.html

files=$(ls -1)
来源：http://hz.havefunace.top/gtwdlposrm.html

[R38] 管道串联
来源：http://hz.cqqwz.cn/gtoscidjnz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yongpay.top/gteiwxanyu.html

[R39] 重定向标准输出与错误
来源：http://hz.mhx1999.top/gtgmeljkvd.html

cmd > out.log 2>&1
来源：http://hz.jqgufenzy.top/gtqdkwvzwf.html

[R40] 追加写日志
来源：http://hz.zycfv.cn/gtqnmznocd.html

echo "log" >> out.log
来源：http://hz.redwolf501.top/gtndjuzrae.html

[R41] 丢弃输出
来源：http://hz.feifeiyinyue.top/gtjgccncey.html

cmd >/dev/null 2>&1
来源：http://hz.jyoumei.cn/gtivwlvyhs.html

[R42] 输入重定向
来源：http://hz.zhaomingkeji.xyz/gtkkcqckki.html

wc -l < a.txt
来源：http://hz.shangyingyoupin.top/gtppnlelet.html

[R43] 按名字查找文件
来源：http://hz.vqdsnc.cn/gtnxeczxhv.html

find . -name "*.log" -type f
来源：http://hz.xingfuxueyuan.xyz/gtwsyxzusy.html

[R44] 按修改时间查找
来源：http://hz.316326.xyz/gtzxxmrirh.html

find . -mtime -7 -type f
来源：http://hz.xuetiantiany.cn/gthljvssid.html

[R45] 批量删除
来源：http://hz.hywenlv.cn/gtvstkdnpw.html

find . -name "*.tmp" -delete
来源：http://hz.hnqzz.top/gtuqvaipld.html

[R46] 递归替换文件内容
来源：http://hz.wangshuangyany.cn/gttxhlclcr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.gotoacloud.top/gtrtizjygx.html

[R47] sed 单行替换
来源：http://hz.yanxiufei.cn/gtpbcpfwku.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hnxiangtu.top/gtfmowarhv.html

[R48] awk 取指定列
来源：http://hz.snrcjt.cn/gtdhskbqnp.html

awk '{print $1, $3}' a.txt
来源：http://hz.pengpengdd.cyou/gtwbgugtlz.html

[R49] awk 带条件
来源：http://hz.hnqzz.top/gtrwujscdl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.guannengcc.top/gtbbpfpdsd.html

[R50] awk 求和
来源：http://hz.yj20258.top/gttfpdgltu.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.snrcjt.cn/gtdscyhbhh.html

[R51] 排序去重取前几
来源：http://hz.hnxiangtu.top/gtqalnfvcx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yongpay.top/gtqplqecpu.html

[R52] 统计行数
来源：http://hz.yuxming.cn/gtkusvrqxr.html

wc -l a.txt
来源：http://hz.yuanzhike.top/gtmnrcjkbo.html

[R53] 查看文件头与实时尾
来源：http://hz.ywan-chungtsiang.top/gtmnxybyhd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.snrcjt.cn/gttzvxoevz.html

[R54] 比较两个文件
来源：http://hz.mhx1999.top/gtrffvnkym.html

diff a.txt b.txt
来源：http://hz.hammf.cn/gttdjlpwxt.html

[R55] 压缩与解压
来源：http://hz.aizwys.cn/gttpulwsvh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.cucudq.cn/gtfyxiykmq.html

[R56] 远程拷贝
来源：http://hz.cucudq.cn/gtrkudznbd.html

scp file user@host:/path/
来源：http://hz.jqgufenzy.top/gtzyerwigf.html

[R57] 远程执行命令
来源：http://hz.daria6918.cn/gtmrpkppvd.html

ssh user@host 'uptime'
来源：http://hz.chenzaomai.com/gtdztrpvfp.html

[R58] 下载文件
来源：http://hz.vqdsnc.cn/gtgpewcvor.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yonumen.top/gtuxppetlv.html

[R59] 发 POST JSON
来源：http://hz.ywan-chungtsiang.top/gtxfjkyfub.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.316326.xyz/gtpomyodto.html

[R60] 只看 HTTP 状态码
来源：http://hz.hfpthk.cn/gtahnqploq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.snrcjt.cn/gtnaqevnif.html

[R61] 磁盘占用
来源：http://hz.jinqigfzy.top/gtnqlapnji.html

df -h;  du -sh *
来源：http://hz.vqdsnc.cn/gtypuxxcha.html

[R62] 找最占空间的文件
来源：http://hz.havefunace.top/gtjzfkghca.html

du -ah . | sort -rh | head -10
来源：http://hz.hfpthk.cn/gtezehmoug.html

[R63] 内存与进程
来源：http://hz.guannengcc.top/gtsjcjqrcd.html

free -h;  ps aux | grep nginx
来源：http://hz.cheryme.top/gtlrkpcrup.html

[R64] 结束进程
来源：http://hz.birdmap.top/gtmzrpaten.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhixingplan.top/gtgqzsquvr.html

[R65] 查看端口占用
来源：http://hz.ppjwa.cn/gtpgtgzzwm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.mhx1999.top/gtzylrtrtu.html

[R66] 定时任务
来源：http://hz.c1oappe.top/gtkfeptdfj.html

crontab -e;  crontab -l
来源：http://hz.haohaochexian.top/gtsjncpumk.html

[R67] 生成随机十六进制串
来源：http://hz.hywenlv.cn/gtoctrhkjh.html

openssl rand -hex 16
来源：http://hz.zdqjudy.top/gtfrsiljrh.html

[R68] 计算文件校验值
来源：http://hz.zhiwuduotai.top/gtjlyaxanv.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.iojbl.cn/gtiwbcoxeq.html

[R69] 生成随机密码
来源：http://hz.ehwqpu.com/gttsllozpa.html

head -c 16 /dev/urandom | base64
来源：http://hz.xuetiantiany.cn/gteeyjvwaz.html

[R70] 时间戳与互转
来源：http://hz.sxryk.cn/gthtzdefkl.html

date +%s;  date -d @1700000000
来源：http://hz.meibo888.top/gtzwbijowi.html

[R71] 日期格式化
来源：http://hz.yj202588.top/gtrrkbkgnb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zhiwuduotai.top/gthemswltv.html

[R72] 等待端口就绪
来源：http://hz.cqqwz.cn/gthzakrbft.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jqgfzy.top/gthczpjzhl.html

[R73] 分割大日志
来源：http://hz.ybcxt.top/gtnbdfpkig.html

split -l 1000 big.log part_
来源：http://hz.zhijiandao.cn/gtkmcugqvv.html

[R74] 批量重命名
来源：http://hz.birdmap.top/gtmyjmpqjo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hammf.cn/gtcrzgusjy.html

[R75] 导出环境变量
来源：http://hz.ehwqpu.com/gtvtlrfyhs.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ehwqpu.com/gtyetytrng.html

[R76] 使用临时文件
来源：http://hz.wangdashe.top/gtckfjsdvd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.9152youxi.cn/gthbrmorxq.html

[R77] 读取用户输入
来源：http://hz.ydzc1.top/gtlefdwswo.html

read -rp "请输入: " ans
来源：http://hz.yueranfly.top/gtwqfaivxs.html

[R78] 交互式菜单
来源：http://hz.c1oappe.top/gtuxxlczrt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shangyingyoupin.top/gtvhdajwrh.html

[R79] 解析命令行选项
来源：http://hz.meibo888.top/gtxnjjizvp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.gaohongyu789.top/gtielwfqwf.html

[R80] 查看脚本执行耗时
来源：http://hz.svipenyu.cn/gtlgetbjoe.html

time ./run.sh
来源：http://hz.chenlongwang.top/gtzugzwmzi.html

================================================================================
来源：http://hz.wangdashe.top/gtpcldceqz.html

S. C / C++ 专题
来源：http://hz.jianghu66.top/gtpigxcbya.html

================================================================================
来源：http://hz.jyoumei.cn/gtkwxfvmcv.html

[S01] C：Hello World
来源：http://hz.shanyushiyangtech.top/gtpyzjrbqs.html

#include <stdio.h>
来源：http://hz.jqgufenzy.top/gtqonnufth.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cheryme.top/gtqozfctjp.html

[S02] C：变量与格式化输出
来源：http://hz.ydzc1.top/gtoopwuaun.html

int a = 10; printf("%d\n", a);
来源：http://hz.xingfuxueyuan.xyz/gtvyogscto.html

[S03] C：读入整数
来源：http://hz.bjfxy.top/gtvovxkpfb.html

int x; scanf("%d", &x);
来源：http://hz.daria6918.cn/gtvzjttumr.html

[S04] C：字符串复制
来源：http://hz.guannengcc.top/gtucipurcq.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hysaishi.cn/gtytzzpykj.html

[S05] C：字符串长度
来源：http://hz.c1oappe.top/gtrvprxwdn.html

strlen(s)
来源：http://hz.zhoulong.xyz/gtlylqulil.html

[S06] C：字符串比较
来源：http://hz.pycfn.com/gtibvkfbim.html

strcmp(a, b) == 0
来源：http://hz.gogol.net.cn/gtorjugdul.html

[S07] C：数组遍历求和
来源：http://hz.shanyushiyangtech.top/gtjbebvhtk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zycfv.cn/gtqzwmvpwd.html

[S08] C：动态内存分配与释放
来源：http://hz.shuidangran.top/gtukmdnwhv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.tian-w.cn/gtxdqiuuva.html

[S09] C：结构体定义与初始化
来源：http://hz.guowangkeji.top/gtlnczlduj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhaomingkeji.xyz/gtcxlqkubh.html

[S10] C：指针与解引用
来源：http://hz.gotoacloud.top/gtwmuqcxut.html

int *p = &a;  *p = 5;
来源：http://hz.tian-w.cn/gtlqtuekxh.html

[S11] C：逐行读文件
来源：http://hz.redwolf501.top/gtxldceypu.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jinqigufen.top/gtvmicmgig.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jinyuanbaomall.cn/gtjnqpbtrq.html

fclose(f);
来源：http://hz.ivvv.top/gtwgbpoccc.html

[S12] C：写文件
来源：http://hz.zhoulong.xyz/gtiftpevnk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.gzhubu.top/gtdocoofvm.html

[S13] C：宏定义
来源：http://hz.cucudq.cn/gtyjpggwfd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ybcxt.top/gtixuzcngo.html

[S14] C：枚举
来源：http://hz.yj20258.top/gtsumxlhqf.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jiagoushi.top/gtynsqcwnb.html

[S15] C：类型转换
来源：http://hz.zycfv.cn/gtooobfvra.html

(double) a / b
来源：http://hz.aizwys.cn/gtxkyhswnk.html

[S16] C：位操作置位
来源：http://hz.dashuyun.cn/gtfwuydzdb.html

x |= (1 << 3);
来源：http://hz.jinyuanbaomall.cn/gtonifhnuf.html

[S17] C：安全拼接字符串
来源：http://hz.hfpthk.cn/gtvstswfpl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yueranfly.top/gtzaypipdd.html

[S18] C：命令行参数
来源：http://hz.zycfv.cn/gthfruhlbg.html

int main(int argc, char **argv)
来源：http://hz.chenlongwang.top/gtgdgyufzg.html

[S19] C：快速排序
来源：http://hz.nanxuanxn.top/gtjgkhuwji.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hongshengwenyu.top/gtsoyexysf.html

[S20] C：二分查找
来源：http://hz.bjfxy.top/gtuecldmtk.html


<!-- 参考信息 -->