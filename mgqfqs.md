代发 wailian999

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3lfwgupzy.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3csdtvpee.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3xcmvutpj.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3eoqppark.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3kknpuibt.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3pdnsdatw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3idvpjrzn.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3awdbsvfv.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ljqcryig.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3sivpieee.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3xrhschnz.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3skwuumqo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ysuveniw.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3epbnuzkr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ymekczzs.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3jnvmmzng.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3wfbrcojh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3rtaerhah.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3xbkhlden.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3swnirpqs.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3kdhzywff.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ymlrwrvy.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3pdknalez.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3mycdugje.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3grhpxiai.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rvxtzpco.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3shqiscli.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3temzgcqc.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3jcnscbum.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bhfywdjj.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3upueipgv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bbzveaqc.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3okhapfeo.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lyvmczfm.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3fosijdwa.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ncmayyed.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3smmvpovr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3kvzxyfah.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3cnaysuww.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3yhlmwtef.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3riqmqbhd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3hjhpbzfe.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pyxlldly.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3thheuext.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3eutuffhz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3vctmspru.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3kkbpsgme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aqowgohc.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3gtdpsajf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tomepbhz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3wyhhewye.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3aqvfsnvk.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3xsaxdkuu.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3zqkrnhte.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3nkrppphh.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3rplignpt.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ukikfoui.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3vkrtwdcv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3kpxjwaju.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3efcyutab.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ybucrqpr.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3rasjvbjv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3sbdyfpmj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3bcgkqnfb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ntjyhyzw.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3pnsqwdje.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ahixjkuz.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nrgkvqzk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3faaqnbkx.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lrdwjpna.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3guyawsrt.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3uwazweuj.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3nxbqwvsu.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jpsdglev.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3yyzbszdw.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3skbspmyu.html

esac
来源：http://www.52xcode.cn/Article/details/gt3hcwybnlc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3lihvgoeo.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3wvymyxai.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3vpetqdcx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3odaxbefa.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3fkzoorpk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3phqjsmaj.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xepwpfnt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nyiatwmf.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3spxiysip.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3pdxuapxg.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3alhejlmu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3pcyinlft.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3hrxlnmwx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cwyzqfci.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3nlvckvgy.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3efvfljgw.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3vqxupkwj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3tbnugchf.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3kfefyziz.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ytpywyuq.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3kkwdchdd.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3yzbqkeyt.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3enofozfa.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3qjmifgdj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3otudzouy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3wqvsctcc.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3jfuduvff.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3dguflcrx.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3cznnnfno.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3nnfwoaqh.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3rqzudqxj.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3arruzmtk.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3vvkznayx.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3fppgriin.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3wnoxtaak.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3epqdgqqt.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3hilfdfre.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3bhzmchyz.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3vqjkvsll.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3verfbaov.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3vgkyqusn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvvsyvpi.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ctbqwlhq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ultyhntp.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ozrdlrit.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3zbjlfixc.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3tgvcvsgq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3gpsbtnkt.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ejzipfdt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3zzjldegv.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3goqpepip.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3zzbcjyqs.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3dypqnwlp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3tmthfzug.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3pdpamkgr.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3hhfmnjky.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3snbcebya.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3jfitcgsw.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3lleulbjl.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3dbakmjvf.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3cwnequpf.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lnjmnhbb.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3xoqbpsbl.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3floskodn.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3cbhbijea.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3shfjnlft.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3hbxxuksu.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3qdzorkhv.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3baxxenyk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3djyvmies.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3tijbcmin.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cfmbvqtq.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3fjxlawrl.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wojumtkj.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3metxxslx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3nbprjulc.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3scenvdcb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3txswlvww.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3rdistlsx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3jfhmvwnh.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3szjgfkhx.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wvuvnint.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3oguhdpbx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3kesuezvy.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3jwyutplm.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3vdpngorz.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3yvrawzth.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3vvithiug.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3axxiuxbk.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3mnjoirlb.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3lwiqntah.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3sgdokpow.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3imypuana.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3gryngnwc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ymxxvypq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3wecgxwmq.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zbeuyhyf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3blfwqtif.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3veoggwcv.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3xfllfvbp.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3pjlezbqi.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3oqfeefvm.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3mudfltdt.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3dodlafth.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3yewhgues.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3lwotgfjl.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3ldxatvbk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3inuclcsz.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3xhusiidq.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3kvqwvuzn.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3ksfgrsts.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3masqzvoc.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3qwcssntj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jvknwbnk.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3yaavkgje.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3huoeluma.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3mabhlfje.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3thzrwssc.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3stgdvkpn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3qxdmxrtb.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3bcthxlvc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3frsheyqh.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3bzdwyopm.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3zcspevci.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3tqdbifrj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wmrzwshq.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3fwyfxmwq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3bmfswlwh.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3mxegkpic.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xtdhcwge.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3mhskysrp.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3ablwhqhf.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3jmpehkhc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3rabqszzc.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3ezsdoxaz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3kfvxvbdt.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3iniaqoee.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ewslboot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rjydfhbh.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ptpbhmtj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oastofzt.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hdgxsbyv.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3onesleff.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3lhzfunjg.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3mqfscoub.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3kulqgxan.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3qvccrmkl.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3heibwlzn.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3uotmcduh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3irzaopkr.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3pulvzyya.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zrwahiyo.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tyesbzaf.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3mokywdxz.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3xactcdfn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3pccwdarl.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3wxoeiypx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ikumvzkw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3pusxnuxy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3imkjrctk.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3eyiqefbi.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3yjkkgzqr.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zsbegnet.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ccunhhcr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ugxzwfvv.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3yzdofnnw.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3rywqbsqu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3pbcqlgon.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3hkdcgxzg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3erlzfrtl.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3cnmdswfp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3kkyfleus.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3vffrzkly.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3pvnoqowy.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3smvmeoat.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lzgfcavq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3humiahaq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3siogtsvu.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3vrsekznr.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3gppwtjin.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3mrocyxzs.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gmwhdhaz.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ojzytdqf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bavyqwih.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3titfvoyd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ttwzlegd.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3fxujoolx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3wfvkcbtk.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3dxwfmiam.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3cpzvhsve.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3myubduhq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3yvbxaemr.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3qjfujdqe.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3wpkvxmof.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3yhdjnzml.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3euimgoox.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3lczuyllp.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pyypdzmp.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3yhldyrls.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3kajrszgz.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3qkthgbvm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3mogdxsmb.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3nunluetq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3tmbeumka.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3kqcunkin.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3mtnimmnx.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3udidstpw.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3krtcufmd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3bbglyqmi.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3mtjtqtlo.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ioopnsih.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ztlyasek.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3swvtxnue.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3llegkooc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3urcvfqlh.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3gmodhjxl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3eoioscig.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3tloardpv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vianpxhg.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3bpsvssph.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gdsbeqmh.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3cshhfxpd.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3joxvrbzh.html


<!-- 参考信息 -->