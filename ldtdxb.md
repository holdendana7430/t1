代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lxcozlhz.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3vmdbmhye.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3bteukvts.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lsgcnllr.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3axhvmmhl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hqrawnuq.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3maysiyfb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bziwbpvq.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3jckpupoo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3qgnrlftp.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3pfhdmweu.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3wxildevr.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ieowlhjp.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3nfvgsako.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3syouizuh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3edkwwglb.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3wcmegyhn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3dnxsaefj.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3xitphwuy.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ojokceiz.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ugbzuxlo.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3qegdkooj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3dwgtmkvs.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3htrlabzh.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3gucoeavw.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3jcwjvpao.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3yadzzgai.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3swmnowok.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ytopputi.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3uldesetd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3qxzpohct.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3qzwdkzzg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3uqafsgul.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cneafurc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jzxuwjkm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3qjgjtanq.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3rgbqjgmw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3brawpivb.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3icweupru.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3hafqeegi.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3gboehadj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3jiuscajv.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3tapscrkh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3rshzpoxj.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3tswxwftz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pxqszsiw.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3qjhcsday.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pfncqfoh.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ngsliyjr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zdgcotxu.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ratvlcfw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aafkpstb.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3wxxsqkrm.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wiwmpwsa.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3okwnvbai.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ugxnelgc.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3wzphmsne.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3cdubfdoe.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3vfzhljoc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3jwsiajbb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ivfbgvwk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3pyjbnddh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iffebqkj.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3loumkkla.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3axjutjlh.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3pvlrbxzq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3wpmeuxzq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3szhywlal.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ncxvfydm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vhacmyfo.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3wjsrxdmi.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3eojusxji.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3skngdvmv.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3oceebelj.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3qgwennrt.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3yhqjuamt.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3fvzsejmm.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3llmlskjn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3oyccvigr.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ihgotonz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3mrhcytkf.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3cvheckwd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqilreen.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3khpxibgb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3edladjuw.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3hhcepssl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dkoduxbq.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vuulhdox.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xduufxaf.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3pawecfqy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lcpmozhg.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3vgggcolm.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3loavxgqm.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3fboyjrjo.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3alaubccv.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xxgwsdxa.html

esac
来源：http://www.52xcode.cn/Article/details/gt3qagabjba.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3yjjqvnfl.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ugrjjalk.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3mncwreao.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ojejfhbv.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3uizylbpz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3qoncjyuf.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rnfijuln.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3toiajvpq.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3yzepptng.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ggckzupc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3aegwkgwc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3quvmbqjf.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3syrcwgbk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3gyehrwbk.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3dihhmuix.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3tachmror.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3musxjyea.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ucyokrzr.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3fdhzvmsd.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3uvzcmdgo.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3kwpqgcpo.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3cbfjgwoq.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3zxjtupis.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3fxbedvxu.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vbatyoeo.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3lqhlrtsn.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3elieujnf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3qxrxodzo.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3sfjjsbjq.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3fcshyccx.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3ezelabkk.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3biyhvlpt.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3mmngaovy.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3rnfcbiwz.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3hvhlwpkh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3fsopvvfc.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3dvmvrvcw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3yoeghmnt.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3moutgtbj.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3vmyheotz.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3wjylglwd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3migfufik.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3cclwrwts.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3gmhvaaoj.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3tflxglrf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3conrzaba.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3sqevkodo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3xhbpzrnm.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3zdghmgya.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3zrxhfajl.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3jqjlwvbx.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3kpdyzrcq.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3hujsmovg.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3pvkjiurs.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3rmjnhfww.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ciuwohau.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3enbjshws.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3nxychhjw.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3yswnwxfy.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3nvnxvrjc.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3jrguzxns.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3gkdkrvoj.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3kroeuotj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3sojqming.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3fffxaulk.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ehznfxnc.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3blweabqi.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3fpdaxbbk.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3wanxlagk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3xwaawzrf.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3bmhfjdex.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qkegyfou.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3kufvrpyw.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cugomcit.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3jrqmbakq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3czrjdzzq.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3rqoarrhl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bymilzeu.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3gxvepeka.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3jvyudrgo.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3dmpsnolp.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hrrixakn.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ylsixzxm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3umfzvoaj.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ojrniwni.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jgnjxckz.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3fuvtzgng.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3isjecvna.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3yymuzvcp.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3kxdxaabw.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3qwvsyrhl.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3giikktap.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3flhgpeyp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3unzwfjwn.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mwrpgndl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ymeyraqq.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3iysernpt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3ltiymhqs.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3hnlukwjf.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3plpqdbsg.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3khylenii.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3unjtwdkh.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3rvivzgjv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3jupguhmj.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3hwotbnds.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3gmoojglj.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3sbqgfcbw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3gfuibbnr.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3aompdplc.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3vyqmbdfz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3uqprwgyd.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3jcbvanqq.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3gkkqxetw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tykumilf.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3krdjlkkk.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3djcmwmcc.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3usxtbcud.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3iroahzak.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pbwyacix.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ypstroax.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3qimzmuvf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3jsithfwa.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3eksvkwjo.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ulelhyqf.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3hdtedmmy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3zwkoomor.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3sihflgvn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3azvalibq.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ssbfnjfu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3snhasmld.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3vncmgbzx.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3ilmiafuk.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3iuakbfmx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3puhfnrnt.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3ljwjsbpx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3djxrbggj.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3jprpbxjy.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3qhlcazcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bfmtklqx.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3nqmojmox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rukjgskg.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qyexjgco.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3kasljpon.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3tstwhrgs.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3hpkrekrf.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3ahuvbiqf.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3wuxfrjgm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3fvqsnrvx.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ximvtxyk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3hchwycgq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3wqllkepp.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3wgnjtpup.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3mxqoushj.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3qrpdexpa.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3qobpftpi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3fqolxmqh.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ossodwaa.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3uxcwkztc.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3nxyqhulp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3sguutvxz.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3cgyqplhr.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ywonphws.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fbquxkyv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3qdrhrscl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3wpvlewhs.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3jhgswdmx.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3phkorrwn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3mpquoeas.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3dtbzmnlj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3jzfqzhxy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qjtoczrl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3miiahsmn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3xbqsnebw.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3uxncwrxg.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3rtibcvys.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3hnluuwvo.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3bexccqnj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3cqjzabes.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3dqcqwovt.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3icgsdvmt.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3cjqeagpb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vhfnpkoz.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3eisidcyw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3apwvwfcu.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3rqhyjrrq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3jxfvqrdr.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3hsywmicv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3jqoybuli.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3jnoshbcp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3wzmrypnf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3dvnqtrbi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3yyjjrnrt.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ihaxihij.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3soplksyw.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3xrnravtb.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3rbmryypq.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3ndgfxqoj.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zsngkdca.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3rkoobsct.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3svjecaxn.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3nztemdos.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3yffcvlid.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3aafhlwrg.html


<!-- 参考信息 -->