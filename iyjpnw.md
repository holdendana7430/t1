代发 wailian999

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3fsoxarxy.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3vdfwrxuq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3tfovbgwa.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3fmxvlvqy.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3eshqnyph.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3jhgqausx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3epqawmoc.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3cpohbhwi.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fnvtrpnd.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3putwyovi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3gwfyyrqw.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ofbgcgsk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3yxptjazu.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ajxluxve.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3igoecwul.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3xgbknfif.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3nrmfjdmc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3hfkzaiiw.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3lnswmzmp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3fcmiepli.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3pxjdtejy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ozzcidta.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3pdohyofb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3extxqdhe.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3wtpkwimo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gtpkvgdn.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3oltywwax.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ukkpsidc.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3abtjowuz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ytfgdkwl.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hqvfgvmj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gkjqvnbl.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3cfjdrvds.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xawrhgsc.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ztgvvlke.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3tuvpfuzc.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3vuxagmvu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3bjxwngyu.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3bilwwiyo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3uxyajwyg.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3lptdcywz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3mmyupfit.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vbrzcskv.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3qfuxbauf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3vvmrgdmw.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3jcjmpgkk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3avuhirce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uhgcmopk.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3tknlfvcp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zvunpnvp.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3eqqsoyes.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3oobhgpan.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3xamfyvkl.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3hxflyjnh.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3dtssqmee.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3yblhcmux.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3jgpmmkbw.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3typkewes.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ihqpxdjv.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3gbszhvko.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3iczhywac.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3oqxxkgnu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrcqkfht.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3onrninmb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3acqaqmve.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3iaeynent.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xtsffwmd.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gskgwuht.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3klqdkkoi.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3drkpqqkx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uohxktat.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3sgbmyjdd.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3czzchujx.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3zdfkobhg.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3hvjibxnf.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ltfivtan.html

esac
来源：http://www.52xcode.cn/Article/details/gt3vkrjncsp.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3pwotrbbx.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hgdryzul.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3tcvknoys.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ogbgcbwh.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3vnzvhnoy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3obekfnch.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3thfidflg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3ermhkedi.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3tqiiefrs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3tbjpvjct.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ttbpcoeq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3csnngfwr.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3puxalyae.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3yeqmuzhe.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3fluusfhd.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3sfcpctel.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3yawbmvhf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3yybckaho.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qzbztdnq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3bpnsfxmf.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3iwssxrkk.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3xfsizjzh.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3qnyuevzv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3tdepokve.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jrkkckct.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3bvehkxsg.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3vtyizzpn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ryjhkltb.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3uyjdhvpr.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3oolniwbm.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3kynywras.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3vsxzrgom.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3gtaonhig.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3zcoodwxg.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ympmbbzi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3rrvdfsdm.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3mddvmegc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3kjdsyrzp.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3iiixlypr.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ylrtupgw.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3pkfzlhul.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3elgbxjix.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3eklcyckk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3chzypiry.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3nrniweoi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3qdmfzctl.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3ghksitvz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3auyesagh.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3yldfbatm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3osgnwsfw.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3fdtkvdit.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3vysmvacn.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3nitnkyyr.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3jxsltiho.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3jgnqeiqa.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3epaeidcq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3uaskszdy.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3xquzqnrz.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ryppyaqp.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3oowoggnd.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3aogpdqsu.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nirhpevk.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3uvyldyde.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3kqjdckyg.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3uoofyawg.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3naslyeag.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3ksdpdynv.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3gbmcegaz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3gdkdepyd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3hkbywtxs.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3jmmbttuo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qiiwaibd.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3rzrsoqrs.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bovjbazl.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3llcrjjaw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3cwfgrhzq.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3naqwqxrb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mltmalwt.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3megqystc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3vslrbuzl.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3heqxivze.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jafpunij.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3dglxnvuc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ddrdspvi.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3kejaxjnj.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wcfmweah.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3cfcidodt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3nejaooef.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fmdflzlc.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3efcmvems.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3jpyyqvug.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3aknjcudx.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3rywxxboz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3tmnpgdok.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3oxnvfcuj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3bemkxdke.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3usnffots.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3mecrbfpz.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3nbvlddpi.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3bukmejeo.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3jsgnikuz.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3sduhbrwq.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3xoglhfha.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3qirsiyle.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3tueiojny.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3fzyacxpk.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3qqqfaovj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3yjbilxkz.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3geoqoupk.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3dxsgnlex.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3acywwsyp.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3szvfbkdm.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3ifjdqzem.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3xzyxevgq.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3okmkjbqi.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3pknghioz.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ugzlckyh.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3nhjzdvaj.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lzrcujyk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3gljjdlcg.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3nnhrtbqq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3oczhunle.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3fkrqyoya.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3twsdogop.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ymtavlin.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3xdlpyhqu.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3vlcnsmbb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3zhddiudc.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3qqteybbq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3tftwkumi.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3eieagthd.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3xegknrha.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3zpsnzvxr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3mminhkej.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3vjghcode.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3gsiiqkdl.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3dixbliym.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ghjfqwgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dmogbras.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3bnpjfmmu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tcvinory.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ftvpgveh.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3jztqxiwy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3xatmomwo.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3rjtppyqe.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3iqxztysu.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ytewjapg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3repoltuz.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3obybpxzf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3mqsdjfef.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3hoolxxnv.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kftcbjtr.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3gpvlxyyn.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3yjoycquw.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3kmrrizcq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3mteqicrw.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3gwhjpskj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3yffmrjnf.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3glbihapf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ggwweohd.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3bkmisdba.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3jfgfjiiu.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ktlqmukm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3pbhkvhnk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3bbjkmewq.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3cmtpkxvy.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3reodlkdj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3hzxxulvx.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3dnitjjqa.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3uvizefwy.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ccxcitmp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3lwqvixgd.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3bnwnobjw.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3scaxpuft.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3hijxvvxd.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ttexhheo.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tgtljzvx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3buvjpuzr.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3goovjygv.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3kmirppxf.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3fieybdgw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jcgcyxqn.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3govhmszy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zvbgotis.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3bcldlssh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3rtnhlkfw.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3lswbrixb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3weqzwbll.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3fwvnaoqx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ayjzzibe.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3bkuxesjk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3znacrfup.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3xhnqolel.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3ypnigixe.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3fevfawbn.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3fhbymtrj.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3okstorky.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hkwguzuc.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3wkillioy.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3fvtxyjse.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3fncnhliv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3rycfuixx.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3wdjibyig.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3zlauqgpw.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3sqinetcl.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3evopmute.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hqxdhbbq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3acqltypn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3xckutveq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ivejcavi.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3wxvsevqq.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3oadarbrf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3akddwhrd.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3nsutjnmg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3gzbhwynl.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3niyjxwts.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gtqkborr.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3zpdyvshb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kesqxfhw.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3rjgdapgh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3aiwddhjc.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3dnqjzrth.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3bzbiuxzo.html


<!-- 参考信息 -->