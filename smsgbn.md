代发 wailian999

[Q48] CTE 公用表表达式
来源：http://hz.birdmap.top/gtpinseorx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.snrcjt.cn/gtmksgbreu.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.smart0.xyz/gtjqjaudir.html

[Q49] 更新单行
来源：http://hz.dianchejie.cn/gtvkoyrpqv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.pycfn.com/gtjblimkce.html

[Q50] 批量更新
来源：http://hz.yj202588.top/gtwhuybtdh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.tian-w.cn/gtizkvoute.html

[Q51] 用子查询更新
来源：http://hz.tian-w.cn/gtiizosrpj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhijiandao.cn/gtlnikrrzr.html

[Q52] 删除指定行
来源：http://hz.xylfe.cn/gtqwwhuwws.html

DELETE FROM users WHERE id = 10;
来源：http://hz.sxryk.cn/gtbjxzyark.html

[Q53] 按条件删除
来源：http://hz.yj20258888.top/gtcvwuzfkb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hywenlv.cn/gtvridekjx.html

[Q54] 清空表
来源：http://hz.zhixingplan.top/gtkbgabjoa.html

TRUNCATE TABLE logs;
来源：http://hz.yj20258.top/gtdtnsepzz.html

[Q55] 排名（并列占位）
来源：http://hz.cucudq.cn/gtvcgjdkyq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.daxiang520.top/gtjdbyeywa.html

[Q56] 密集排名（并列不占位）
来源：http://hz.pengpengdd.cyou/gtihvmyepx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.dianchejie.cn/gtmpidvzub.html

[Q57] 行号
来源：http://hz.tian-w.cn/gtfvfzhoxc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhongyouzk.top/gtdxjivfzk.html

[Q58] 累计求和
来源：http://hz.mhx1999.top/gtqvjjmwyi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.nanxinkj.top/gtveyomorr.html

[Q59] 分组内累计
来源：http://hz.jinghuilouyu.cn/gtmdylydpr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hammf.cn/gtbrzmboso.html

[Q60] 取上一行 / 下一行
来源：http://hz.cdnleiting.top/gttzagkczc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yueranfly.top/gtzgmmxirp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hysaishi.cn/gtigldyafo.html

[Q61] 移动平均
来源：http://hz.fengsongda.top/gtdexiycse.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.sweek.top/gttxykdwaw.html

[Q62] 分组占比
来源：http://hz.wangdashe.top/gtioubtrbn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hnxiangtu.top/gtvfkdfxoa.html

[Q63] 开启事务
来源：http://hz.yonumen.top/gtfybhansq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.andypj.xyz/gtxyopnoip.html

[Q64] 提交事务
来源：http://hz.haohaochexian.top/gtxkepzmsi.html

COMMIT;
来源：http://hz.yanxiufei.cn/gtfpztqxmn.html

[Q65] 回滚事务
来源：http://hz.cucudq.cn/gtifbjcocx.html

ROLLBACK;
来源：http://hz.ppjwa.cn/gtcioujxwu.html

[Q66] 行锁查询
来源：http://hz.jinyuanbaomall.cn/gtsszlcsju.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hywenlv.cn/gtxhoblvkx.html

[Q67] 设置隔离级别
来源：http://hz.shanyushiyangkeji.top/gttoldxkvm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.nanxuanxn.top/gtjeaspagr.html

[Q68] 保存点
来源：http://hz.ppjwa.cn/gtvrvblxpw.html

SAVEPOINT sp1;
来源：http://hz.xylfe.cn/gtiwbulfyt.html

ROLLBACK TO sp1;
来源：http://hz.cqqwz.cn/gtpesupfqe.html

[Q69] 查看执行计划
来源：http://hz.jqgufenzy.top/gtplcmkpyq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xziqi.cn/gtedvlihhe.html

[Q70] 更新统计信息
来源：http://hz.316326.xyz/gtoyesxlyv.html

ANALYZE TABLE users;
来源：http://hz.9152youxi.cn/gteroeyrns.html

[Q71] 查看建表语句
来源：http://hz.mhx1999.top/gtfgtuamel.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.svipenyu.cn/gtispzofmo.html

[Q72] 查看索引
来源：http://hz.ydzc1.top/gtvkvzygbf.html

SHOW INDEX FROM users;
来源：http://hz.vqdsnc.cn/gtuhsjwtfc.html

[Q73] 查看表状态
来源：http://hz.daxiang520.top/gtlmkntior.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.birdmap.top/gtiutoprqr.html

[Q74] 强制使用索引
来源：http://hz.gaohongyu789.top/gtmvxqmepx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.dashuyun.cn/gtmascqsyh.html

[Q75] 日期格式化
来源：http://hz.cqqwz.cn/gtnpgjlutc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhixingplan.top/gtukabanak.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ydzc1.top/gtccivrmge.html

[Q76] 按天统计
来源：http://hz.tianlin.xyz/gtickrhdwc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.kuanghao11.cn/gtretvtvil.html

[Q77] 时间加减
来源：http://hz.yj202588.top/gtlutffbpn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.mhx1999.top/gtxvuqzxyk.html

[Q78] 当前时间
来源：http://hz.jqgufenzy.top/gtfgoynhjh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jqgufenzy.top/gtsdpuqmpz.html

[Q79] 字符串拼接
来源：http://hz.xinyue.icu/gtdncdvwda.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.birdmap.top/gtcuzxjkcz.html

[Q80] 字符串截取
来源：http://hz.yangfankeji.com/gtpaxitfsj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.shangyingyoupin.top/gtxmatqjsg.html

[Q81] 字符串替换
来源：http://hz.gogol.net.cn/gttmcwgffd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yuxming.cn/gthfjxyyif.html

[Q82] 字符长度与字节长度
来源：http://hz.yonumen.top/gtnioquhlx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ydzc1.top/gtckzgqbjg.html

[Q83] 大小写转换
来源：http://hz.chenlongwang.top/gtthcgoypk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.andypj.xyz/gtaytukmin.html

[Q84] 去除首尾空格
来源：http://hz.yangfankeji.com/gtqjkccsei.html

SELECT TRIM(name) FROM users;
来源：http://hz.tianlin.xyz/gtfdowxrge.html

[Q85] 数值取整
来源：http://hz.jinyuanbaomall.cn/gtvqgqpubm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yvedp.cn/gttbncdqjr.html

[Q86] 读取 JSON 字段
来源：http://hz.wangshuangyany.cn/gthcnxgpjx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yueranfly.top/gtpzbfzmis.html

[Q87] JSON 字段做条件
来源：http://hz.xuanzx.com/gtxbzordvt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.aizwys.cn/gtakacoefi.html

[Q88] 行转列（条件聚合）
来源：http://hz.xinyue.icu/gtfqsrflki.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.quarkkingdee.top/gtgsymzjgh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ywan-chungtsiang.top/gthkocggvu.html

[Q89] 判断表是否存在
来源：http://hz.jqgufenzy.top/gthguaqeyx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yongpay.top/gtyajxaibf.html

[Q90] 生成序号列
来源：http://hz.zdqjudy.top/gtbiwvczps.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hywenlv.cn/gtjmlaebqn.html

================================================================================
来源：http://hz.gogol.net.cn/gtvpnpygdl.html

R. Bash 专题
来源：http://hz.aizwys.cn/gtetcbhabg.html

================================================================================
来源：http://hz.gaohongyu789.top/gtdkipkqbz.html

[R01] shebang 与严格模式
来源：http://hz.ydjk.org.cn/gtfdvxgwzw.html

#!/usr/bin/env bash
来源：http://hz.jqgufenzy.top/gtholnmtrj.html

set -euo pipefail
来源：http://hz.c1oappe.top/gtpepiixcb.html

[R02] 变量赋值与使用
来源：http://hz.birdmap.top/gtvlyxbwlt.html

name="Tom"; echo "$name"
来源：http://hz.zhengqikj.top/gtcvlcfiqc.html

[R03] 只读变量
来源：http://hz.shanyushiyangtech.top/gtfsmtgdrg.html

readonly PI=3.14
来源：http://hz.xylfe.cn/gtelehznog.html

[R04] 位置参数
来源：http://hz.xziqi.cn/gtxbjtvezj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.sweek.top/gtjakbyuoe.html

[R05] 参数默认值
来源：http://hz.316326.xyz/gttpgbmkug.html

name="${1:-default}"
来源：http://hz.zdqjudy.top/gtjgqogzsd.html

[R06] 判断命令是否存在
来源：http://hz.wangshuangyany.cn/gtqijnbzei.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shzxlz.cn/gtojuknkud.html

[R07] if 判断文件
来源：http://hz.jianghu66.top/gtjijekeid.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yuanzhike.top/gthkzxzgrs.html

[R08] 数值比较
来源：http://hz.cashguo.top/gtizhsmhhc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhixingplan.top/gtwqtseqrj.html

[R09] 字符串比较
来源：http://hz.ivvv.top/gtgbylbcvx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.fengsongda.top/gtwyfglpww.html

[R10] 正则匹配
来源：http://hz.9152youxi.cn/gtmcdkpqwn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.quarkkingdee.top/gtzwmvdnuo.html

[R11] case 多分支
来源：http://hz.yj202588.top/gtwznsjlet.html

case "$1" in
来源：http://hz.fengsongda.top/gtamdfwzxt.html

start) echo "启动" ;;
来源：http://hz.nwbrower.top/gtlagqutze.html

stop)  echo "停止" ;;
来源：http://hz.yangfankeji.com/gtexbuljfp.html

*)     echo "未知命令" ;;
来源：http://hz.9152youxi.cn/gtqgqhasdo.html

esac
来源：http://hz.yuxming.cn/gthxenldgz.html

[R12] for 遍历文件
来源：http://hz.sysykeji.top/gtmzuwclbz.html

for f in *.txt; do echo "$f"; done
来源：http://hz.svipenyu.cn/gtepglzfll.html

[R13] for 计数循环
来源：http://hz.yuxming.cn/gteucqkdog.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yuanzhike.top/gtbhrfjorj.html

[R14] C 风格 for
来源：http://hz.yvedp.cn/gtzmqjwspi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.fengsongda.top/gtxvsafoiz.html

[R15] while 逐行读文件
来源：http://hz.zdqjudy.top/gtkudbvndt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yj20258888.top/gtplddlucg.html

[R16] until 等待条件
来源：http://hz.jqgfzy.top/gtkoixxzrf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.haohaochexian.top/gtgbdhvmez.html

[R17] 数组定义与取值
来源：http://hz.gotoacloud.top/gtsfkqtvzj.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xinyue.icu/gtdwmsreyx.html

[R18] 遍历数组
来源：http://hz.birdmap.top/gtaqtgkfnu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hfpthk.cn/gtkkjrbrfu.html

[R19] 数组长度
来源：http://hz.daxiang520.top/gtccnrkpgn.html

echo "${#arr[@]}"
来源：http://hz.ywan-chungtsiang.top/gtluxrdffs.html

[R20] 关联数组（字典）
来源：http://hz.shuidangran.top/gtjjxhdxmj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hnqzz.top/gtedebegpw.html

[R21] 字符串长度
来源：http://hz.cdnleiting.top/gtlyhbhkyj.html

echo "${#s}"
来源：http://hz.aibaodan.cn/gterfibsys.html

[R22] 截取子串
来源：http://hz.sxryk.cn/gtkrpazeqy.html

echo "${s:0:5}"
来源：http://hz.hysaishi.cn/gtglxlhucp.html

[R23] 字符串替换
来源：http://hz.jqgfzy.top/gtlnyujjsk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ehwqpu.com/gtyznrljgl.html

[R24] 大小写转换
来源：http://hz.yuxming.cn/gtmriducos.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yj202588.top/gtnfcnqgff.html

[R25] 去后缀 / 去前缀
来源：http://hz.tanke756.top/gtbqvzzlak.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hnxiangtu.top/gtestkdpnr.html

[R26] 命令替换
来源：http://hz.yj202588.top/gtuzyudmve.html

now=$(date +%F); echo "$now"
来源：http://hz.shanyushiyangtech.top/gtnypnocei.html

[R27] 算术展开
来源：http://hz.ywan-chungtsiang.top/gtwxppkfmk.html

echo $((1 + 2 * 3))
来源：http://hz.zhengqikj.top/gtkmukwtym.html

[R28] 浮点运算
来源：http://hz.redwolf501.top/gtneivzrvy.html

echo "scale=2; 10/3" | bc
来源：http://hz.yangfankeji.com/gtrezjilee.html

[R29] 定义函数
来源：http://hz.hywenlv.cn/gtiynaipbg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yonumen.top/gtskwuftzw.html

[R30] 函数返回状态码
来源：http://hz.zhijiandao.cn/gtnzibsvdr.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jiagoushi.top/gtchpklsoc.html

[R31] 局部变量
来源：http://hz.fzhhl.top/gtpvjnnyyh.html

f() { local x=1; echo "$x"; }
来源：http://hz.fengsongda.top/gtznipyhej.html

[R32] 参数个数校验
来源：http://hz.sweek.top/gtjwkbdmyf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hfpthk.cn/gtxwkzjmmy.html

[R33] 捕获错误并提示行号
来源：http://hz.jqgfzy.top/gtdhqpiouz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.tian-w.cn/gtfhcsayow.html

[R34] 退出时清理
来源：http://hz.jinqigfzy.top/gtosqouuxd.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.shanyushiyangtech.top/gtvclpotag.html

[R35] 后台执行并等待
来源：http://hz.daxiang520.top/gtodvmwusg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hnqzz.top/gtlraltseh.html

[R36] 并发执行多个任务
来源：http://hz.zdqjudy.top/gtvwkjmyhn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.gzhubu.top/gtnickblgy.html

[R37] 把输出赋给变量
来源：http://hz.redwolf501.top/gtndzztboc.html

files=$(ls -1)
来源：http://hz.c1oappe.top/gtogqxkejv.html

[R38] 管道串联
来源：http://hz.jqgufenzy.top/gtnvlfjzup.html

cat a.txt | grep -i error | wc -l
来源：http://hz.52xcode.cn/gtptgwnzxv.html

[R39] 重定向标准输出与错误
来源：http://hz.ydzc1.top/gtxkxipxkm.html

cmd > out.log 2>&1
来源：http://hz.wangdashe.top/gtromwudzl.html

[R40] 追加写日志
来源：http://hz.jinqigfzy.top/gtxppmenge.html

echo "log" >> out.log
来源：http://hz.quarkkingdee.top/gtppiqoxfi.html

[R41] 丢弃输出
来源：http://hz.kuanghao11.cn/gtzcjzbvnk.html

cmd >/dev/null 2>&1
来源：http://hz.shangyingyoupin.top/gtgeweaoyz.html

[R42] 输入重定向
来源：http://hz.nanxuanxn.top/gtbnafbbzq.html

wc -l < a.txt
来源：http://hz.gzhubu.top/gtkcidewai.html

[R43] 按名字查找文件
来源：http://hz.redwolf501.top/gtplbtvwbb.html

find . -name "*.log" -type f
来源：http://hz.fengsongda.top/gtkpmxkaud.html

[R44] 按修改时间查找
来源：http://hz.ydjk.org.cn/gtvcallcio.html

find . -mtime -7 -type f
来源：http://hz.ybcxt.top/gtzwiwlbif.html

[R45] 批量删除
来源：http://hz.yongpay.top/gtdxbfqfuc.html

find . -name "*.tmp" -delete
来源：http://hz.yangfankeji.com/gtunfoqsct.html

[R46] 递归替换文件内容
来源：http://hz.yvedp.cn/gtrwplkyro.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yuxming.cn/gttrhkkxgb.html

[R47] sed 单行替换
来源：http://hz.zhongyouzk.top/gtqictdlvk.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.dashuyun.cn/gtexiftfmo.html

[R48] awk 取指定列
来源：http://hz.pycfn.com/gtuphdzuqi.html

awk '{print $1, $3}' a.txt
来源：http://hz.aizwys.cn/gtsfqopazo.html

[R49] awk 带条件
来源：http://hz.sysykeji.top/gtqxzxbnsz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.kuanghao11.cn/gtgsvmnnsg.html

[R50] awk 求和
来源：http://hz.iojbl.cn/gtgljivasf.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.gogol.net.cn/gtbzrooaga.html

[R51] 排序去重取前几
来源：http://hz.kuanghao11.cn/gtnxcfepck.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.birdmap.top/gtixwpaxpc.html

[R52] 统计行数
来源：http://hz.jyoumei.cn/gtfgitdwxx.html

wc -l a.txt
来源：http://hz.shanyushiyangkeji.top/gtxbdpjuvj.html

[R53] 查看文件头与实时尾
来源：http://hz.cucudq.cn/gtcnvjegsv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yonumen.top/gtqwqljstd.html

[R54] 比较两个文件
来源：http://hz.jiagoushi.top/gtsgoybwxl.html

diff a.txt b.txt
来源：http://hz.chenjidiqi.icu/gtsyuhucgk.html

[R55] 压缩与解压
来源：http://hz.ydzc1.top/gtrmiwevrc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.sxryk.cn/gtscjrjbul.html

[R56] 远程拷贝
来源：http://hz.zhiwuduotai.top/gthagbxgsc.html

scp file user@host:/path/
来源：http://hz.daria6918.cn/gtjtvepaee.html

[R57] 远程执行命令
来源：http://hz.hnqzz.top/gtgwwdibjs.html

ssh user@host 'uptime'
来源：http://hz.yuxming.cn/gtdelyvoqz.html

[R58] 下载文件
来源：http://hz.yuxming.cn/gtyamcbfyy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.chenzaomai.com/gtdgplwjbw.html

[R59] 发 POST JSON
来源：http://hz.yj20258.top/gtekhdeqza.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shzxlz.cn/gtjzwkouti.html

[R60] 只看 HTTP 状态码
来源：http://hz.jqgufenzy.top/gtubzketfh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ydjk.org.cn/gtynhtyswl.html

[R61] 磁盘占用
来源：http://hz.kuanghao11.cn/gtztwdjnuu.html

df -h;  du -sh *
来源：http://hz.chenjidiqi.icu/gtlidtgmby.html

[R62] 找最占空间的文件
来源：http://hz.dashuyun.cn/gtiwqfyick.html

du -ah . | sort -rh | head -10
来源：http://hz.havefunace.top/gtgmskyuka.html

[R63] 内存与进程
来源：http://hz.52xcode.cn/gtzfanorcr.html

free -h;  ps aux | grep nginx
来源：http://hz.jqgfzy.top/gteayeyzto.html

[R64] 结束进程
来源：http://hz.iojbl.cn/gtukeynpec.html

kill -9 $(pgrep -f app.py)
来源：http://hz.redwolf501.top/gtsqpjzufv.html

[R65] 查看端口占用
来源：http://hz.daxiang520.top/gtdnulirze.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.kuanghao11.cn/gtksdbabhs.html

[R66] 定时任务
来源：http://hz.cucudq.cn/gtleuylqlc.html

crontab -e;  crontab -l
来源：http://hz.fengsongda.top/gtzrnvhfql.html

[R67] 生成随机十六进制串
来源：http://hz.zhixingplan.top/gtjernfzsx.html

openssl rand -hex 16
来源：http://hz.yj202588.top/gtpqppsgfm.html

[R68] 计算文件校验值
来源：http://hz.wangdashe.top/gttvmxrfew.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cucudq.cn/gtginpllpb.html

[R69] 生成随机密码
来源：http://hz.pengpengdd.cyou/gtdkmdhyhl.html

head -c 16 /dev/urandom | base64
来源：http://hz.xuanzx.com/gtqyyclrty.html

[R70] 时间戳与互转
来源：http://hz.sufxvd.cn/gtqruzuuem.html

date +%s;  date -d @1700000000
来源：http://hz.birdmap.top/gtrxgqjsxl.html

[R71] 日期格式化
来源：http://hz.ydzc1.top/gtjvcnutez.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.redwolf501.top/gtsmujxbzh.html

[R72] 等待端口就绪
来源：http://hz.shanyushiyangtech.top/gtjwrygidk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jinqigufen.top/gtdsmkplxo.html

[R73] 分割大日志
来源：http://hz.gotoacloud.top/gtrczhtntj.html

split -l 1000 big.log part_
来源：http://hz.ydjk.org.cn/gtgmlvinmx.html

[R74] 批量重命名
来源：http://hz.hammf.cn/gtygopmdam.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.cheryme.top/gtivfvjhcv.html

[R75] 导出环境变量
来源：http://hz.zhongyouzk.top/gtxvxvuqsx.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.gotoacloud.top/gtrrrhasun.html

[R76] 使用临时文件
来源：http://hz.chenjidiqi.icu/gtmaqgcguf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinyuanbaomall.cn/gtayvoalfu.html

[R77] 读取用户输入
来源：http://hz.zhixingplan.top/gtqnwgvdbj.html

read -rp "请输入: " ans
来源：http://hz.feifeiyinyue.top/gtqhdfjisf.html

[R78] 交互式菜单
来源：http://hz.tianlin.xyz/gtekkmqdsi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.wangdashe.top/gtzeinthvd.html

[R79] 解析命令行选项
来源：http://hz.ppjwa.cn/gtrpivflyv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.vqdsnc.cn/gtgrjcoihe.html

[R80] 查看脚本执行耗时
来源：http://hz.zdqjudy.top/gtbwufjipa.html

time ./run.sh
来源：http://hz.dianchejie.cn/gtmumexkqc.html

================================================================================
来源：http://hz.sufxvd.cn/gtzmigtgal.html

S. C / C++ 专题
来源：http://hz.tanke756.top/gtwygnlzjj.html

================================================================================
来源：http://hz.ydjk.org.cn/gtflkqhwrl.html

[S01] C：Hello World
来源：http://hz.jinqigfzy.top/gtssjrsnft.html

#include <stdio.h>
来源：http://hz.hfpthk.cn/gtrshwnqyc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.nwbrower.top/gtooqachro.html

[S02] C：变量与格式化输出
来源：http://hz.cucudq.cn/gtszydvrcr.html

int a = 10; printf("%d\n", a);
来源：http://hz.yuanzhike.top/gtqbfqfhjk.html

[S03] C：读入整数
来源：http://hz.xuanzx.com/gttumyjcue.html

int x; scanf("%d", &x);
来源：http://hz.zhoulong.xyz/gtpoqtgnfu.html

[S04] C：字符串复制
来源：http://hz.fengsongda.top/gtsgbcxvnl.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jinqigufen.top/gtcsaabvyw.html

[S05] C：字符串长度
来源：http://hz.sysykeji.top/gtxgbiccem.html

strlen(s)
来源：http://hz.sysykeji.top/gterrrzfvi.html

[S06] C：字符串比较
来源：http://hz.gzhubu.top/gtegeoxovr.html

strcmp(a, b) == 0
来源：http://hz.jinghuilouyu.cn/gtptxfmtyh.html

[S07] C：数组遍历求和
来源：http://hz.gotoacloud.top/gtatfsybqr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yueranfly.top/gtzjdmwuue.html

[S08] C：动态内存分配与释放
来源：http://hz.ydzc1.top/gtaulradns.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinyuanbaomall.cn/gtbfdbtsgg.html

[S09] C：结构体定义与初始化
来源：http://hz.mhx1999.top/gtyqtakrbm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jinqigufen.top/gtrskgykza.html

[S10] C：指针与解引用
来源：http://hz.nanxuanxn.top/gtbtrksuia.html

int *p = &a;  *p = 5;
来源：http://hz.shanyushiyangkeji.top/gtavgirxry.html

[S11] C：逐行读文件
来源：http://hz.daria6918.cn/gttzrdeegl.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.bjfxy.top/gteaxteohn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hysaishi.cn/gtxojykqbi.html

fclose(f);
来源：http://hz.aibaodan.cn/gtnzvirtlz.html

[S12] C：写文件
来源：http://hz.ivvv.top/gtucugojyo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.aizwys.cn/gtvcpuncvo.html

[S13] C：宏定义
来源：http://hz.guannengcc.top/gtqxxmicjk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.shanyushiyangtech.top/gtsdlyroyd.html

[S14] C：枚举
来源：http://hz.shangyingyoupin.top/gtuqtjmvwi.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.birdmap.top/gtzommfoqg.html

[S15] C：类型转换
来源：http://hz.aibaodan.cn/gtnokfuwer.html

(double) a / b
来源：http://hz.jinyuanbaomall.cn/gtlfacjgxu.html

[S16] C：位操作置位
来源：http://hz.meibo888.top/gtossaoigr.html

x |= (1 << 3);
来源：http://hz.hysaishi.cn/gtizcbpowg.html

[S17] C：安全拼接字符串
来源：http://hz.guannengcc.top/gtyzbkypql.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jinqigufen.top/gtzhpcklgu.html

[S18] C：命令行参数
来源：http://hz.zhijiandao.cn/gtkartirie.html


<!-- 参考信息 -->